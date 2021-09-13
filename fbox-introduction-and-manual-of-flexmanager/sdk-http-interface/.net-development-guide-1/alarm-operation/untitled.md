# Obtain All the Alarm Entries under FBox

```text
/// 
/// Obtain all the alarm entries under FBox
/// 
/// 
public IList GetAlarmItems()
{
    var allitems = _fbox.GetAllAlarmDefinitionsV2(new BoxArgs()
    {
        BoxNo = boxNo
    }).Result;
    foreach (var items in allitems)
    {
        Console.WriteLine(items.TaskState);    //Entry state
        Console.WriteLine(items.AlarmGroup);   //Alarm grouping 
        Console.WriteLine(items.AlarmMessage); //Alarm information
        Console.WriteLine(items.Code);         //Alarm entry coding 
        Console.WriteLine(items.Condition1);   //Alarm condition 1
        Console.WriteLine(items.ConditionCombineMethod);//Condition combination
        Console.WriteLine(items.Id);            //Alarm entry Id
        Console.WriteLine(items.IsDeviceChanged);//Whether the equipment has been changed
        Console.WriteLine(items.Memo);          //Remark
        Console.WriteLine(items.Name);          //Alarm entry name
        Console.WriteLine(items.Operand1);      ////Operand, if bit data type is selected, operand 0 is OFF, 1 is ON
        Console.WriteLine(items.Condition2);    //Alarm condition 2
        Console.WriteLine(items.Operand2);      //Operand
    }
    return allitems;
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
                fbox.GetAlarmItems();//Call this method 
            }
        }
    }
```

