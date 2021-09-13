# Box Status Change Cush

## Box status change push <a id="&#x76D2;&#x5B50;&#x72B6;&#x6001;&#x53D8;&#x66F4;&#x63A8;&#x9001;"></a>

When the server detects a status change of FBox, it will push a message The message content is an array The attributes of a single object are as follows

| Field name | Type | Parameter Description |
| :--- | :--- | :--- |
| id | string | the ID of FBox |
| state | int | The current status of the box, 0: unknown, 1: connected, 2: timed out, 3: disconnected |
| net | int | Box network type 1: Network 2: 2G, 3: 3G \(currently not supported\) 4: WIFI, 5: 4G |
| rssi | int | Signal: 0~8 |
| vers | json Object | FBox firmware version，fcs，fds,floader. |
| mode | int | FBox status 0：normal，1：Transparent transmission |

## Listen for events <a id="&#x4FA6;&#x542C;&#x4E8B;&#x4EF6;"></a>

```text
/// 
/// Start
/// 
public void Start()
{
    // Log in to the server via parameters
    _fbox.Restart().Wait();
    //Listen to box state change events
    _fbox.BoxConnectStateChanged += _fbox_BoxConnectStateChanged;
}
//Called in the Program，Main function
    {
        static void Main(string[] args)
        {
            using (var fbox = new FBoxDemo())
            {
                fbox.Start();  //Start
                fbox.StartAllDMonData();//Turn on all the monitoring points of box
            }
        }
    }
```

```text
/// 
/// Box state change function
/// 
/// 
/// 
private void _fbox_BoxConnectStateChanged(object sender, IList e)
{
    foreach (var stateItem in e)
    {
        Console.WriteLine($"{stateItem.BoxNo},{stateItem.NewState}");
    }
}
```

