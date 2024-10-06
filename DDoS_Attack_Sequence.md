sequenceDiagram
	participant Attacker
	participant BotNet
	participant WebServer
	participant Firewall
	Attacker->>Botnet: Traffic generator
	Botnet->>Webserver: UDP Flood
	Firewall->>Webserver: Block traffic
	
	1. The attacker sends program to bots on the botnet.
	2. All of the bots on the botnet floods the Webserver with UDP data packets.
	3. The firewall tries to block inbound traffic from IP addresses thare are reserved, loopback, private, unassigned DHCP clients,
	   multicast and experimental.