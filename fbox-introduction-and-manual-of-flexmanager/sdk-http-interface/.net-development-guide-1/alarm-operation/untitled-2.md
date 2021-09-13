# New Alarm Entry

```text
/// 
/// New alarm entry
/// 
public void AddAlarm()
{
    _fbox.AddAlarmDefinitionV2(new AddAlarmDefArgsV2()
    {
        AddAlarms = new List()
        {
            new AddAlarmDefinitionV2()
            {
                Name = "Alarm name",        // The name of the new alarm entry is unique and cannot be the same name
                DevAlias = "Modbus_TCP", //The device driver alias
                StationNo = 1,          //PLC communication station number
                DataType = DataType.Bit, //Data type, see appendix 2 in the interface document for details
                RegName = "4X_bit",    //register name, and regId, iowidth determine the only register
                //The address should be configured according to the monitoring point that the alarm entry needs to detect
                MainAddress = 8, //Main address
                SubAddress = 0,//Sub-address
                SubIndex = 0,//DB block address
                AlarmMessage = "XXXX",  //Alarm information
                GroupName = "Alarm grouping", //Alarm point group name or use GroupId alarm group Id, priority name
                Memo = "",             //Remark
                //The below are the alarm condition
                Condition1 = AlarmConditionType.Eq,//Trigger alarm condition type, alarm condition 1, 0: not equal to, 1: equal to, 2: greater than, 3: greater than or equal to, 4: less than, 5: less than or equal to
                Operand1 = 80,  //Condition value
                ConditionCombineMethod = AlarmConditionCombineMethod.And, //Conditional union, None: None, And: And, Or: Or
                Condition2 = AlarmConditionType.Eq,//Trigger alarm condition type, alarm condition 1, 0: not equal to, 1: equal to, 2: greater than, 3: greater than or equal to, 4: less than, 5: less than or equal to
                Operand2 = 90 //Condition value
            }
        },
        BoxNo = boxNo     //The Box number of the new alarm entry
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
                fbox.AddAlarm();//Call this method
            }
        }
    }
```

