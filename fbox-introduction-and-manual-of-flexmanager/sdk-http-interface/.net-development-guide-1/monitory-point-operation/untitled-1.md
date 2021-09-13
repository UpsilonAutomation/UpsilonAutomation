# Update Monitoring Point Entry

## Update Monitoring Point Entry <a id="&#x66F4;&#x65B0;&#x76D1;&#x63A7;&#x70B9;&#x6761;&#x76EE;"></a>

After the monitoring point is added, you need to connect to SignalR successfully, and then turn on the monitoring point data push

```text
/// 
/// Update Monitoring Point Entry
/// 
public void UpdateDmon()
{
    _fbox.UpdateDataMonitorPointV2(new UpdateDmonArgsV2()
    {
        BoxNo = boxNo,//Box number
        UpdateDmonList = new List()
        {
            new UpdateDataMonitorDefinitionV2()
            {
                Id = 113470726140747285,//The ID of the new entry to update
                GroupName = "fff",//The name of the monitoring point group, and the groupId can be used. If a non-existing monitoring point group is used, the group will be automatically added
                Name = "ggg",//Monitoring point name 
                DevAlias = "Local",//PLC alias
                StationNo = 1,//Station number
                DataType = DataType.Int16,//Data type, see appendix 2 in the interface document for details
                RegName = "LW",//register name, and regId, iowidth determine the unique register
                //Please fill in the address according to the configuration of the device
                MainAddress = 9,//Main address
                SubAddress = 0,//Sub-address
                SubIndex = 0,//DB block address
                IntegralDigits = 0,//Integer bits (No effect so far)
                FractionalDigits = 1,//Decimal bits
                Unit = "Degree",//Unit
                Privilege = PrivilegeType.ReadOnly,//Read and write permissions，2：Write,4：ReadOnly,6：ReadWrite,
                TrafficSaving = true,//Whether to enable the data-saving mode, true: enable, false: not enable
                DeadValue = 15,//Dead zone value, data will not be pushed within the range of ±deadValue
                BitStateLabel =  new BitStateLabel(),//Display label when bit type, attribute ttext: the text displayed when the value is 1, ftext: the text displayed when the value is 0
                Memo = "ggg",//Remark
                Encoding = EncodeType.None//Encoding format, string type use 0: None, non-string type use, 1: Unicode, 2: Ascii
            }
        }
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
                fbox.StartAllDMonData();//Open FBox all the monitroing points
                fbox.UpdateDmon();//Call this method
            }
        }
    }
```

## **Delete Monitoring Point Ent**ry <a id="&#x5220;&#x9664;&#x76D1;&#x63A7;&#x70B9;&#x6761;&#x76EE;"></a>

```text
/// 
/// Delete monitoring point entry
/// 
public void RemoveDmon()
{
    List ids = new List { 113470815205744205 };
    _fbox.RemoveDataMonitorPointV2(new RemoveDataMonDefArgsV2()
    {
        BoxNo = boxNo, //Box number
        Ids = ids      //Id collection of monitoring point entry to be deleted
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
                fbox.RemoveDmon();//Call this method
            }
        }
    }
```

