# Obtain Historical Record Entry

```text
/// 
/// Obtain historical record entry
/// 
public void GetHdataList()
{
    var itemlist =  _fbox.GetHdataItems(new BoxArgs()
    {
        BoxNo = boxNo                                       //Box number
    }).Result;
    foreach (var items in itemlist)
    {
        Console.WriteLine(items.BoxId);                     //Box Id
        foreach (var channels in items.Channels)
        {
            Console.WriteLine(channels.Uid);                //Channel Id
            Console.WriteLine(channels.HasSubAddress);      //Does the register have a subaddress
            Console.WriteLine(channels.HasSubIndex);        //Does the register have a DB block address
            Console.WriteLine(channels.DataType);           //Data type, see appendix 2 in the interface document for details
            Console.WriteLine(channels.MainAddress);        //Main address
            Console.WriteLine(channels.RegName);            //Register number
            Console.WriteLine(channels.RegId);              //Register Id
            Console.WriteLine(channels.IoWidth);            //Register bit width
            Console.WriteLine(channels.StationNo);          //Station number
            Console.WriteLine(channels.SubAddress);         //sub-address
            Console.WriteLine(channels.DevAlias);           //PLC alias
            Console.WriteLine(channels.SubIndex);           //DB block address
        }
        Console.WriteLine(items.Name);                      //Name
        Console.WriteLine(items.RecordingPeriod);           //Collection cycle
        Console.WriteLine(items.Uid);                       //Main key
        Console.WriteLine(items.IsControl);                 //Whether to use enable
    }
}
//Called in the  Program，Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start
                fbox.StartAllDMonData();//Open FBox all the monitoring points
                fbox.GetHdataList();//Call this method
            }
        }
    }
```

