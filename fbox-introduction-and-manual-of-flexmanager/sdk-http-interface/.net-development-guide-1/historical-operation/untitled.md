# Obtain Historical Record Multi-Channel Data

```text
/// 
/// Obtain historical record multi-channel data
/// 
public IList GetHdataHistory()
{
    var hdata =  _fbox.GetByRowHistoryData(new GetHistoryDataArgs()
    {
        BoxNo = boxNo,                                //Box number
        StartTime = DateTime.Parse("2018-06-06 08:58:32"),       //starting time
        EndTime = DateTime.Parse("2018-06-07 08:58:32"),        //End time
        Limit = 500,                                 //Maximum number of data obtained
        TimeRange = TimeRangeTypes.BeginOpenEndOpen, //Interval type,BeginCloseEndClose:全毕区间,BeginCloseEndOpen:左闭右开，BeginOpenEndClose:左开右闭，BeginOpenEndOpen:全开区间
        HdataItemName = "XX",                        //Historical data entry name
        HdataChannelNames = new List() { "11", "22"}//Channel name
    }).Result;
    foreach (var d in hdata.Rows)
    {
        Console.WriteLine(d.Time); // Collection time of historical data entries
        Console.WriteLine(d.Values[0]); // Corresponds to the first element in the channel name set
        Console.WriteLine(d.Values[1]); // Corresponds to the second element in the channel name set
    }
    return hdata.Rows;
}
//Called in Program, Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start
                fbox.StartAllDMonData();//Open FBox all monitoring point
                fbox.GetHdataHistory();//Call this method
            }
        }
    }
```

