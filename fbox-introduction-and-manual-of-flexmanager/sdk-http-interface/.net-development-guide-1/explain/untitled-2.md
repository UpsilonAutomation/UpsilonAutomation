# Open All Monitoring Points of the Specified FBox

Enable all monitoring point data push of current online FBox

```text
/// 
/// Turn on all monitoring points of the box
/// 
public void StartAllDMonData()
{
    //After the box is offline, you need to adjust this interface every time you go online
    _fbox.StartAllDataMonitorPointsOnBox(new BoxArgs(boxNo)).Wait();//boxNo is box number
}
//Called in the Program，Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start
                fbox.StartAllDMonData();//Turn on all monitoring points of FBox
            }
        }
    }
```

## **Turn on Monitoring Point Data Push** <a id="&#x5F00;&#x542F;&#x76D1;&#x63A7;&#x70B9;&#x6570;&#x636E;&#x63A8;&#x9001;"></a>

Could turn on the specified monitoring point data push 

```text
/// 
/// Enable monitoring point data push
/// 
public void StartDmonData()
{
    // After adjusting the interface to add a new monitoring point, you need to adjust this interface to receive the data push of the new point
    _fbox.StartDataMonitorPoint(new DataMonitorPointArgs()
    {
        BoxNo = boxNo,                      //Box ID
        DataMonitorUid = 113470726140747285 //Monitoring point Uid
    });
}
//Called in the Program，Main function
class Program
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start
                fbox.StartDmonData();//Turn on monitoring point
            }
        }
    }
```

