# Obtain Box Information and Box Grouping

```text
/// 
/// Obtain Box Information and Box Grouping
/// 
public void GetBoxGroups()
{
    var grpList = _fbox.GetBoxGroups().Result;
    foreach (var grp in grpList)
    {
        Console.WriteLine(grp.Uid);                 // Uid of the box group
        Console.WriteLine(grp.Name);                // box group name
        foreach (var box in grp.Boxes)              // traverse the set of boxes under the group
        {
            Console.WriteLine(box.BoxId);           // Box Id
            Console.WriteLine(box.Alias);           // Box name
            Console.WriteLine(box.BoxNo);           // Box number
            Console.WriteLine(box.ConnectionState); // When getting the box state, it cannot be used as a real-time state, and this interface cannot be called all the time as a box state change. Please use SignalR to push the state change in real time.
            Console.WriteLine(box.NetworkType);     // Network type 1: network, 2: 2G, 3: 3G (this does not support), 4: Wifi, 5: 4G
            Console.WriteLine(box.Disabled);        // Whether the box is disabled
            Console.WriteLine(box.ApiBaseUrl);      // ApiBaseUrl server address
            Console.WriteLine(box.SignalrUrl);      // SignalR server address
            Console.WriteLine(box.Owned);           // Is it the owner
            Console.WriteLine(box.BoxType);         // Box type, 0: standard box, 1: mini box, 2: Lite 3: VPN box
        }
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
                fbox.StartAllDMonData();//Open all the monitoring points of box
                fbox.GetBoxGroups();//Call this method
            }
        }
    }
```

