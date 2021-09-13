# Real-Time Data Push

## Real-time data push <a id="&#x5B9E;&#x65F6;&#x6570;&#x636E;&#x63A8;&#x9001;"></a>

Prerequisite: The monitoring point has been turned on, and the box needs to be reopened every time the box goes offline. When the monitoring point data changes or the monitoring item is turned on, the server pushes a message.

| Field Name | Type | Parameter Description |
| :--- | :--- | :--- |
| boxSessionId | int | Currently negligible |
| values | json array | The value collection of the monitoring point, the details of a single attribute are shown in the table below |
| boxUid | string | the id of FBox |

value corresponding attribute

| Field Name | Type | Parameter Description |
| :--- | :--- | :--- |
| id | string | Monitoring point entry uid |
| value | string | Value, if the entry is configured with decimal places, the program needs to transfer by itself, and the server does not do any transfer |
| status | int | If the entry is normal, there is no such attribute 1: no data, 2: timeout, 3: error, 4: Socket exception, 5: FDS error, 16: not completed |

## **Listen for Events** <a id="&#x4FA6;&#x542C;&#x4E8B;&#x4EF6;"></a>

```text
/// 
/// Start
/// 
public void Start()
{
    // Log in to the server via parameters
    _fbox.Restart().Wait();
    //Listen to real-time data change events
    _fbox.DataMonitorValueChanged += _fbox_DataMonitorValueChanged;
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
            }
        }
    }
```

```text
/// 
/// Real-time data change function
/// 
/// 
/// 
private void _fbox_DataMonitorValueChanged(object sender, IList<DataMonitorValueChangedArgs> e)
{
    foreach (var dmon in e)
        Console.WriteLine($"dmv:{dmon.Uid}:{dmon.Value},{dmon.Status}");
}
```

