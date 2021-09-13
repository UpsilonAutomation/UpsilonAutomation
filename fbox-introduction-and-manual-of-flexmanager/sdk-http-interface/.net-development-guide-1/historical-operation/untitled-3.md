# Update Historical Record Entry

## **更新历史记录条目** <a id="&#x66F4;&#x65B0;&#x5386;&#x53F2;&#x8BB0;&#x5F55;&#x6761;&#x76EE;"></a>

```text
/// 
/// Update historical record entry 
/// 
public void UpdateHdata()
{
    _fbox.UpdateHdataItems(new UpdateHdataItemArgs()
    {
        BoxNo = boxNo,
        HdataItems = new List()
        {
            //The following is an example of updating a channel
                    new UpdateHdataChannelsDto()
                    {
                        Uid = 97427676249298676, //Channel Uid
                        ChannelName = "15",//Channel name
                        DevAlias = "ABB AC500_RTU",//PLC alias
                        StationNo = 2,//Station number
                        DataType =   DataType.Int16,//Data type, see appendix 2 in the interface document for details
                        RegName = "4X",//Register name, confirm the unique register with regId and iowidth
                        //Please fill in according to the device's configuration
                        MainAddress = 7,//Main address
                        SubAddress = 0,//Sub-address
                        SubIndex = 0,//Indexing address
                        Unit = "°",//Unit
                        IntegralDigits = 0,//Integer bits
                        FractionalDigits = 2//Decimal bits
                    }
                },
                IsControl = true,   //Wheter to start enable control
                //When start enable configuration, please configure enable parameter
                ControlOptions = new HDataControlOptionsV2()//Enable parameters
                {
                    ControlType = HControlType.OFF,//Enable states,0:OFF,1:ON
                    DataType = DataType.Bit,  //Data type, see appendix 2 in the interface document for details
                    DevAlias = "ABB AC500_RTU",   //PLC alias
                    StationNo = 2,              //Station number
                    RegName = "0X",             //Register name and regId, iowidth confirm the unique register
                    //Please fill in according to the device's configuration
                    MainAddress = 2,            //Main address
                    SubAddress = 0,             //Sub-address
                    AddressDescription = "ABB",  //Address description
                    BitIndex = 0,               //Bitwise inexing number
                    BitIndexEnabled = false     //Whether to enable bitwise indexing
                },
            }
        }
    });
}
//Called in the Program，Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //start 
                fbox.StartAllDMonData();//Open FBox all the monitoring points
                fbox.UpdateHdata();//Call this method 
            }
        }
    }
```

## **删除历史记录条目** <a id="&#x5220;&#x9664;&#x5386;&#x53F2;&#x8BB0;&#x5F55;&#x6761;&#x76EE;"></a>

```text
/// 
/// Delete historical record entry 
/// 
public void RemoveHdata()
{
    _fbox.RemoveHdataItem(new RemoveHdataItemArgs()
    {
        BoxNo = boxNo,                                  //Box number
        Ids = new List() { 85289974828733605 }    //History record Id collection
    }).Wait();
}
//Called in the Program，Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start
                fbox.StartAllDMonData();//Open FBox all the monitoring points
                fbox.RemoveHdata();//Called this method 
            }
        }
    }
```

