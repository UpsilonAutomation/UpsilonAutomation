# Add Historical Record Entry

```text
/// 
/// New historical record multi-channel 
/// 
public void AddHdata()
{
    _fbox.AddHdataItems(new AddHdataItemArgs()
    {
        BoxNo = boxNo,                          //Box number
        HdataItems = new List()
        {
            //The following is an example of adding a channel, adding multiple channels will increase by itself
                    new AddHdataChannelsDto()
                    {
                        ChannelName = "xxx",    //Channel name 
                        AddressDescription = "LW",//Address description
                        StationNo = 2,          //Station number
                        DataType = DataType.Bcd16,//Data type, see appendix 2 in the interface document for details
                        DevAlias = "Modbus_TCP",  //PLC alias
                        RegName = "4X",        //Register name, confirm the unique register with regId and iowidth
                        //Please fill in according the device's configuration
                        MainAddress = 5,        //Main address
                        SubAddress = 0,         //sub-address
                        SubIndex = 0,           //DB block address
                        BitIndex = 0,           //Bitwise index number
                        BitIndexEnabled = false,//Whether to enable bitwise indexing
                        FractionalDigits = 1,   //Channel decimal places
                    }
                },
                IsControl = true, //Whether to enable control
                //When the enable control is true, fill in the following enable parameters
                ControlOptions = new HDataControlOptionsV2()//enable parameters
                {
                    ControlType = HControlType.OFF,//enable configuration,0:OFF,1:ON
                    DataType = DataType.Bit,    //Data type, see appendix 2 in the interface document for details
                    DevAlias = "Modbus_TCP",    //PLC alias
                    StationNo = 2,              //Station number
                    RegName = "4X_bit",         //Register name, and regId, iowidth determine the unique register
                    //Please fill in according to the configuration of the device
                    MainAddress = 2,            //Main address
                    SubAddress = 3,             //sub-address
                    AddressDescription = "LW",  //Address description
                    BitIndex = 2,               //Bitwise index number
                    BitIndexEnabled = false     //Whether to enable bitwise indexing
                }
            }
        }
    }).Wait();
}
//Called in Program，Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start
                fbox.StartAllDMonData();//Open FBox all the monitoring points
                fbox.AddHdata();//Call this method 
            }
        }
    }
```

