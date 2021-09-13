# Update Alarm Entry

## Update Alarm Entry <a id="&#x66F4;&#x65B0;&#x62A5;&#x8B66;&#x6761;&#x76EE;"></a>

```text
/// 
/// Update Alarm Entry
/// 
public void UpdateAlarm()
{
    _fbox.UpdateAlarmDefinitionV2(new UpdateAlarmDefArgsV2()
    {
        BoxNo = boxNo,//The Box number of the alarm entry
        UpdateAlarms = new List()
        {
            new UpdateAlarmDefinitionV2()
            {
                Id = 113522543645056649,//The Id of the alarm entry
                Name = "edited", //The alarm entry name
                DevAlias = "Modbus_TCP",//the device driver's name 
                StationNo = 1, //PLC communication station number
                DataType = DataType.Int16,//Data type, see appendix 2 in the interface document for details
                RegName = "4X",//register name, and regId, iowidth determine the unique register
                //The address should be configured according to the monitoring point that the alarm entry needs to detect
                MainAddress = 2, //Main address
                SubAddress = 0,//Sub-address
                SubIndex = 0,//DB block address
                GroupName = "Alarm gruoping",//Alarm group name, just use one with groupId
                //The below are the alarming condtion
                Condition1 = AlarmConditionType.Lt,//Trigger alarm condition type, alarm condition 1, 0: not equal to, 1: equal to, 2: greater than, 3: greater than or equal to, 4: less than, 5: less than or equal to
                Operand1 = 12,//Condition value 1, if the Bit data type is selected, operand 0 is OFF, 1 is ON
                ConditionCombineMethod = AlarmConditionCombineMethod.And, //Conditional union, None: None, And: And, Or: Or
                Condition2 = AlarmConditionType.Eq,//Trigger alarm condition type, alarm condition two, 0: not equal to, 1: equal to, 2: greater than, 3: greater than or equal to, 4: less than, 5: less than or equal to
                Operand2 = 90 //Condition value 2
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
                fbox.UpdateAlarm();//Call this method 
            }
        }
    }
```

## **Delete** Alarm Entry <a id="&#x5220;&#x9664;&#x62A5;&#x8B66;&#x6761;&#x76EE;"></a>

```text
/// 
/// Delete alarm entry
/// 
public void RemoveAlarm()
{
    var ids = new List(){ 110424333146494353};
    _fbox.RemoveAlarmDefinitionV2(new RemoveAlarmDefArgsV2()
    {
        BoxNo = boxNo,      //Box number
        Ids = ids           //The UID of the deleted alarm entry 
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
                fbox.RemoveAlarm();//Call this method
            }
        }
    }
```

