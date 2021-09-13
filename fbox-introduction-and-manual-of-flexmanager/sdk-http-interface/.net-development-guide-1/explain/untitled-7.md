# Monitoring Point Value Write

```text
/// 
/// Monitoring Point Value Write
/// 
/// 
public void WriteDmonValue(WriteDmonRequest requet)
{
    _fbox.WriteValue(new DataMonitorWriteValueArgsV2()
    {
        BoxNo = requet.BoxNo,                     //Box number
        DataMonitorGroupName = requet.DmonGrpName,//Monitoring point group name
        DataMonitorName = requet.DmonName,        //Monitoring point entry name
        Value = requet.Value,                     //Vale of entry
        Type = WriteValueType.AutoParse //Entry value type, 0: consistent with the monitoring point value type, 1: decimal, 2: string,
    }).Wait();
}

public class WriteDmonRequest
{
    public string BoxNo { get; set; }
    public string DmonGrpName { get; set; }
    public string DmonName { get; set; }
    public object Value { get; set; }
}
//Called in the Program，Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start 
                fbox.StartAllDMonData();//Open all the monitoring points of box
                fbox.WriteDmonValue();//Call this method
            }
        }
    }
```

