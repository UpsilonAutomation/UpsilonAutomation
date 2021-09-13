# Obtain Box Monitoring Point Grouping and Monitoring Point Entry

```text
/// 
/// Obtain Box Monitoring Point Grouping and Monitoring Point Entry
/// 
/// 
public IList GetDmonGroups()
{
    var dmonGrps = _fbox.GetDmonGroupDmonsV2(new BoxArgs(boxNo)).Result;
    foreach (var grp in dmonGrps)
    {
        Console.WriteLine(grp.Id);          // Id of monitoring point grouping
        Console.WriteLine(grp.Name);        // Name of monitoring point grouping
        foreach (var item in grp.Items)     // Traverse all monitoring point entries under the current group grp
        {
            Console.WriteLine(item.Id);     //monitoring point Id
            Console.WriteLine(item.Name);   //monitoring point name
            Console.WriteLine(item.DevAlias); //PLC alias
            Console.WriteLine(item.StationNo); //Station number
            Console.WriteLine(item.IsDeviceChanged);//Whether the device is removed (this parameter only appears when removing, it is true) This parameter will appear after the FBox connected device is changed
            Console.WriteLine(item.TaskState);  //Entry state
            Console.WriteLine(item.DeadValue);  //Dead value zone
            Console.WriteLine(item.BitIndex);   //Bitwise indexing
            Console.WriteLine(item.BitIndexEnabled);//Whether to enable bitwise indexing
            Console.WriteLine(item.BitStateLabel);//Bit type data tag
            Console.WriteLine(item.CharCount);  //Number of characters
            Console.WriteLine(item.DataType);   //Data type
            Console.WriteLine(item.Encoding);   //Encoding m
            Console.WriteLine(item.FractionalDigits);//Decimal bits
            Console.WriteLine(item.GroupId);    //Monitoring point grouping
            Console.WriteLine(item.GroupName);  //Monitoring point name
            Console.WriteLine(item.IntegralDigits);//Integer bits (currently no effect)
            Console.WriteLine(item.IoWidth);    //Register bit width
            Console.WriteLine(item.MainAddress);//Main address
            Console.WriteLine(item.Memo);       //Remark 
            Console.WriteLine(item.Privilege);  //read and write mode
            Console.WriteLine(item.RegId);      //Register Id
            Console.WriteLine(item.RegName);    //Register name
            Console.WriteLine(item.StringByteOrder);//Byte order
            Console.WriteLine(item.SubAddress); //Sub-address
            Console.WriteLine(item.SubIndex);   //DB block address
            Console.WriteLine(item.TrafficSaving);//Whether to turn on the data saving mode
            Console.WriteLine(item.Unit);       //Unit
            Console.WriteLine(item.ValueTransform);//Data calculation
        }
    }
    return dmonGrps.SelectMany(x => x.Items).ToArray();//Monitoring point entry collection
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
                fbox.GetDmonGroups();//Call this method
            }
        }
    }
```

