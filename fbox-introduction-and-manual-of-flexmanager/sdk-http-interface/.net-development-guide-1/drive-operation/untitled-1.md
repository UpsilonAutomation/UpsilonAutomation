# Download PLC

```text
/// 
/// Download PLC
/// 
public void DownloadPlc()
{
    _fbox.DownLoadPlcsV2(new AddOrUpdatePlcDeviceArgsV2()
    {
        BoxNo = boxNo,
        PlcList = new List()
        {
            //The below is an example of downloading PLC
            //Note that this method will overwrite the previous plc when downloading plc, if you need multiple plc, add it yourself
            new AddOrUpdatePlcDeviceV2()
            {
                PlcId =  305,                       //PLCId
                PlcName = "ABB",                    //PLC alias
                Alias = "ABB AC500_RTU",            //alias
                Type = ServerType.Serial,     //Type，0：serial port，2：Ethernet
                PortNo = 1,                        //serial number
                Class = PlcClass.Master,       //Device type, 0: master device, 1: slave device, 2: master and slave device (currently not supported)
                DefaultStationNo = 1,               //Default station number
                Interface = DeviceInterfaceTypes.Tcp,//serial port interface type，0：RS232，1：RS485_2，2：RS485_4，85：Network (serial port 1 supports RS232, RS485_2 and RS485_4, serial port 2 only supports RS485_2, serial port 3 only supports RS232)
                BaudRate = 9600,                   //Baud rate
                Port = 0,                       //Network device port number
                DataBits = 8,                     //Data bit 
                StopBits = 1,                      //Stop bit 
                ParityType = ParityType.None, //Parity bit，none：No parity, odd: odd parity, even: even parity
                Ip = "0",                        //IP address
                EnableBroadcast = false,      //Whether to start the broadcast station number
                BroadcastStationNo = 0,        //broadcast station number
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
                fbox.StartAllDMonData();//Open FBox all the monitoring points
                fbox.DownloadPlc();//Call this method
            }
        }
    }
```

