# Communication between of Wincc7.4 and FBox through OPC

**Communication between of Wincc7.4 and FBox through OPC**

1. **Required Software**
2. Download OPCServer and FlexManager, download link: [http://fs.flexem.com/Box](http://fs.flexem.com/Box), after downloading and installing, open the FlexManager software to register and log in.

![](../../.gitbook/assets/0%20%286%29.jpeg)![](../../.gitbook/assets/1%20%286%29.jpeg)![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%283%29.jpeg)

1. Settings in flexmanager software. After adding or modifying variables in the flexmanager software, you need to restart the fbox opc Server software to take effect. The data in Opc Sever is synchronized with the flexmanager software. \(If you set it in flexmanager software, please jump directly to the second item\) Add fbox.

![](../../.gitbook/assets/4%20%283%29.jpeg)

1. Add the driver in "Remote Download". The following takes the addition of our FL3 PLC as an example. Click Remote Download-Device Management, add serial port / network port plc.

![](../../.gitbook/assets/5%20%281%29.jpeg)

1. Add the point to be monitored in "Data Monitor", as shown in the following example.

![](../../.gitbook/assets/6%20%286%29.jpeg)

1. **FBox opcserver Software Setting**

Open OPCServer，log in with FlexManager account and password.

![](../../.gitbook/assets/7%20%286%29.jpeg)

1. **Configure Communication Way in wincc**
2. First open or create a new WINCC project, double-click "Variable Manager" to open the variable management interface.

![](../../.gitbook/assets/8%20%281%29.jpeg)

1. Right-click "Variable Management"-"Add New Driver"-"OPC", add a new OPC channel, it will automatically generate an "OPC GROUPS".

![](../../.gitbook/assets/9%20%284%29.jpeg)

1. Right-click "OPC GROUPS" and select "System Parameters" to open the "System Parameters" interface

![](../../.gitbook/assets/10%20%282%29.jpeg)

1. In the "System Parameters" interface, you can see the OPC server on this machine or the network. Select FBoxOpcServer here.

![](../../.gitbook/assets/11%20%281%29.jpeg)

1. After selecting, click "Browse Server". In the pop-up window, check "Read Access" and "Write Access", and select "All Types" as the type.

![](../../.gitbook/assets/12%20%281%29.jpeg)

1. Click Next to view all the variables in the selected OPC server in the pop-up window. Select all the variables you need to communicate and click "Add Entry".

![](../../.gitbook/assets/13.jpeg)

1. Because we have not established an OPC connection before, it will prompt you to create a new connection, click OK, and then modify the OPC connection name.

![](../../.gitbook/assets/14%20%281%29.jpeg)

1. After modifying the name, it will pop up a new window, where we can add the variable prefix and suffix. Here we choose not to add. Click Finish. The communication link between WINCC and the selected OPC server is established. We can directly call the variables in the link in WINCC

![](../../.gitbook/assets/15%20%281%29.jpeg)

Note: wincc software and fbox opcserver software should be run as administrator. And the fbox name and variable name in the flexmanager software are recommended to be in English, Chinese may not be readable

