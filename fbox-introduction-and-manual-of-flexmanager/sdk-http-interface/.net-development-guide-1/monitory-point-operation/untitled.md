# New Monitoring Point Entry

监控点添加完后需要连接SignalR成功后，开启添加的监控点数据推送

```text
/// 
/// New monitoring point entry
/// 
public void AddDMon()
{
    _fbox.AddDataMonitorPointV2(new AddDmonsArgsV2()
    {
        AddDmons = new List()
        {
            new AddDataMonitorDefinitionV2()
            {
                GroupName =  "fff",//The name of the monitoring point group, and the groupId can be used. If a non-existing monitoring point group is used, the group will be automatically added
                Name  = "xxxxx",//Monitoring point name
                DevAlias = "Local",//PLC alias
                StationNo = 1,//Station number
                DataType = DataType.Int16,//Data type, see appendix 2 in the interface document for details
                RegName = "LW",//register name, and regId, iowidth determine the unique register
                Privilege = PrivilegeType.ReadWrite,//Read and write permissions，2：Write,4：ReadOnly,6：ReadWrite,
                //Please fill in the address according to the configuration of the device
                MainAddress =  5,//Main address
                SubAddress = 0,//Sub-address
                SubIndex = 0,//DB block address
                BitIndexEnabled = false,//Whether to enable bitwise indexing
                IntegralDigits = 0,//Integer bits (currently no effect)
                FractionalDigits = 1,//Decimal bits
                Unit = "degress",//unit, only valid for word type
                TrafficSaving = false,//Whether to enable the data-saving mode, true: enable, false: not enable
                BitStateLabel = new BitStateLabel(){FalseLabel = "Turn off",TrueLabel = "Turn on"},//Display label when bit type, attribute ttext: the text displayed when the value is 1, ftext: the text displayed when the value is 0
                Memo = "xxx",//Remark
                DeadValue = 0,//Dead zone value, data will not be pushed within the range of ±deadValue
                //Only inDataType = DataType.String（String type) with the following parameters
                //Encoding = EncodeType.None,//Encoding format, use 0 for string type: None, use for non-string type,1：Unicode,2:Ascii
                //StringByteOrder = StringByteOrder.O12,//String byte order, valid when encoding is in Ascii format 0: reverse order, 1: forward order
                //CharCount = 5, //Number of characters
            }
        },
        BoxNo = boxNo,//Box number
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
                fbox.AddDMon();//Call this method
            }
        }
    }
```

