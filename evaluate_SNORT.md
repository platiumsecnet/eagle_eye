SNORT3
1. Key component plugable

SNORT3 has modular architecture which allows easily extend SNORT3. The most magic capability from this architecture is Snort OpenAppID.
Snort OpenAppID is a plugin which identify approximately 5000 application protocols. It is written on LuA scripts can be easily updated.

2. Rules

An IDS solution is only as good as the available rules it can apply to the monitored traffic. 
Snort has always had a lot of community support, and this has led to a substantial ruleset, updated on a regular basis. 
The syntax of the rules is quite simple, and the program structure allows for anyone to deploy customized rules into their IDS or share them with the community. 
Some commercial parties develop SNORT rules as well, which can be purchased for a monthly or annual fee. 
Some examples are Talos’ SO / VRT rules (released for free after 1 month) and CrowdStrikes Threat Intelligence Services.
Suricata can use the same rules as SNORT. Many, but not all, VRT rules do still work. 
Suricata has its own ruleset, initially released to paying subscribers, but freely available after 30 to 60 days: Emerging Threats. 
These rules make more use of the additional features Suricata has to offer such as port-agnostic protocol detection and automatic file detection and file extraction.

3. Multi-thread

In the past, the main benefits of Suricata over SNORT is multi-thread. However, at the current, SNORT3 also supports multi-thread.
In additional, SNORT3 can process multiple pcap files while SURICATA can only process single pcap file.


4. High Avaibility

The SNORT systems running on appliances in an HA pair inspect packets from mirrored ports. This behavior applies to pairs running in inline protection or inline simulation mode. 
This option decreases the chance of the SNORT systems to miss attacks because the systems analyze all packets, including packets from mirrored ports.