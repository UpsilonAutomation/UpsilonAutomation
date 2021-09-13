# Obtain All the PLC under Box

```text
/// 
/// Obtain All the PLC under Box
/// 
public void GetPlcs()
{
    var boxplc = _fbox.GetPlcDeviceV2(new BoxArgs()
    {
        BoxNo = boxNo                              //Box number
    }).Result;
    foreach (var plc in boxplc)
    {
        Console.WriteLine(plc.Alias);               //plc alias
        Console.WriteLine(plc.BaudRate);            //Baud rate
        Console.WriteLine(plc.BroadcastStationNo);  //Broadcast station number
        Console.WriteLine(plc.Class);//Device type, 0: master device, 1: slave device, 2: master and slave device (currently not supported)
        Console.WriteLine(plc.DataBits);            //Data bit
        Console.WriteLine(plc.DefaultStationNo);    //Default broadcast station number
        Console.WriteLine(plc.EnableBroadcast);     //Enable broadcast station number
        Console.WriteLine(plc.Interface);//serial port interface type，0：RS232，1：RS485_2，2：RS485_4，85：Network (serial port 1 supports RS232, RS485_2 and RS485_4, serial port 2 only supports RS485_2, serial port 3 only supports RS232)
        Console.WriteLine(plc.Ip);        //IP address
        Console.WriteLine(plc.ParityType);//Parity bit, none: no parity, odd: odd parity, even: even parity
        Console.WriteLine(plc.PlcAdvancedSettings); //Advanced settings
        Console.WriteLine(plc.PlcDongleFlag);  //Remote shutdown state
        Console.WriteLine(plc.PlcId);         //PLCId
        Console.WriteLine(plc.SlaveNo);        //the slave device number
        Console.WriteLine(plc.StopBits);     //Stop bit
        Console.WriteLine(plc.PlcName);      //PLC alias
        Console.WriteLine(plc.Type);       //Type，0：serial port，2：Ethernet
        Console.WriteLine(plc.Port);       //Ethernet port number
        Console.WriteLine(plc.PortNo);     //Station number
    }
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
                fbox.GetPlcs();//Call this method
            }
        }
    }
```

