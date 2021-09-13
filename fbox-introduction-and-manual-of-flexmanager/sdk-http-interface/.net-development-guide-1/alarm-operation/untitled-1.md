# Obtain Alarm Historical Record Entry

```text
/// 
/// Obtain alarm historical record
/// 
public void GetAlarmHistory()
{
    var hdata = _fbox.GetAlarmEvents(new AlarmEventQuery()
    {
        BeginTime = DateTime.Parse("2018-4-5"), //Start time long utc timestamp unix epoch
        BoxNo = boxNo,                          //Box number
        EndTime = DateTime.Parse("2018-4-24"),  //End time long utc timestamp unix epoch
        Limit = 500,                            //Get the limit on the number of items, the limit on the number of results. Negative values are for forward query, and 500 is recommended.
        Name = "313265"                         //The code of the alarm entry, if the full search is not required, this parameter is not required
    }).Result;
    foreach (var data in hdata)
    {
        Console.WriteLine(data.Action);         //Type
        Console.WriteLine(data.AlarmId);        //Alarm entry Id
        Console.WriteLine(data.Code);           //Alarm entry code
        Console.WriteLine(data.Message);        //Alarm information
        Console.WriteLine(data.Value);          //Monitoring point value
        Console.WriteLine(data.TimestampUnixEpoch); //Timestamp
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
                fbox.GetAlarmHistory();//Call this method 
            }
        }
    }
```

