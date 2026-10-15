# Ancora-Education-Ucertify-Lab19
# Conducting and Analyzing a SYN flood Using Linux and Windows Server

> **Original Lab Source**
> 
> This lab was available through:
>
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=2]

## Instructions
In this lab, you will learn to conduct and analyze a SYN flood attack using Linux and Windows Server. To conduct and analyze a SYN flood using Linux and Windows Server, here's what you need to do:

1.From the bottom-left bar, click the WIN16 tab. 

2.From the bottom-left bar, click the Ubuntu tab 

3.Navigate to WIN16 tab to perform the further steps. 

4.Click the Start menu and then click Windows Administrative Tools to open the Administrative Tools window. 

5.In the Administrative Tools window, double-click Performance Monitor to open its window. 

6.In the Performance Monitor window, in the left pane, select Performance Monitor.

7.In the right pane of the Performance Monitor window, click the Add icon. 

8.In the left pane of the Add Counters window, under the Available counters section, scroll down, select TCPv4, click Add>> and then click OK. You will see TCPv4 being added under the Added counters section.

9.Minimize the Performance Monitor window and close the Administrative Tools window. 

10.Now, navigate to the Ubuntu tab.

11.If any Software Updater prompt occurs, close it.

12.In the Ubuntu window, from the left sidebar, click Files. 

13.In the Home window, double-click Downloads to open its folder.

14.In the Downloads folder, right-click the netflood.c file and from the context menu, select Copy. 

15.From the left pane, click Desktop, right-click in the blank area in the right pane and from the context menu, select Paste.

16.Minimize the Home window. 

17.From the left sidebar, click the Terminal icon to open its window and execute the following command:
```bash
cd ~/Desktop
```

18.Execute the following command:
```bash
g++ netflood.c -o netflood
```

19.Navigate to the WIN16 tab.

20.On the desktop, click the Search icon, type wireshark to open the The Wireshark Network Analyzer window.

21.In the Software Update dialog box, click Remind me later.

22.In the The Wireshark Network Analyzer window, select Ethernet1, and on the main toolbar, click the Start capturing packets icon.

23.Maximize the Performance Monitor window and observe the performance snap-in. 

24.Go back to the Ubuntu tab and execute the following command in the Terminal window:
```bash
sudo ./netflood 192.168.1.248 192.168.1.1 5003
```

25.If asked for the password enter ucertify.

**NOTE**

The password will not be visible while being typed.

26.Go back to the Performance Monitor window in the WIN16 tab, you'll see multiple spikes in the Performance snap-in.

27.In the bottom pane of the Performance Monitor window, scroll down and observe the results for various objects.

28.Minimize the Performance Monitor window.

29.In the The Wireshark Network Analyzer window, observe the details about source and destination IP addresses.

30.Navigate to Ubuntu tab and press Ctrl+C to stop the SYN flood.

31.Go back to the The Wireshark Network Analyzer window.

32.In the The Wireshark Network Analyzer window, on the main toolbar, click the Stop capturing packets icon and observe the details about various captured packets.

33.Click the Close button to close the The Wireshark Network Analyzer window.

34.In the Unsaved packets window, click Save. In the Wireshark: Save file as window, in the left pane, click Desktop, in the File name textbox, type Wiresharkoutput, and click Save. 

35.Close all windows.

## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.
