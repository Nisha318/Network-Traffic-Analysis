

<h3> TCPDump General Commands </h3>

$ sudo tcpdump

<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump.png">

<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump 2.png">


$sudo tcpdump -c 10 -#A
<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump-c ascii.png">

<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump ascii.png">


$ sudo tcpdump -c 10 -#XX

<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump-c hex.png">


$ sudo tcpdump -c -#tttt

<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump-c human readable.png">

$ sudo tcpdump -D
<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump -D interfaces.png">

$ sudo tcpdump -I ens5 -c 10

<img src="/Analyze Network Traffic with TCPDump/sudo tcpdump -D interfaces2.png">


<h3> Collect Packet Captures in TCPdump using Shell Scripting</h3>

$ sudo tcpdump -#tttt host skyroute66.com -c 10

<img src="/Analyze Network Traffic with TCPDump/skyroute 2.png">

<img src="/Analyze Network Traffic with TCPDump/skyroute 3.png">

$ sudo tcpdump -#xxtttt host skyroute66.com -c 10

<img src="/Analyze Network Traffic with TCPDump/shell script 2.png">









$ sudo tcpdump -#tttt -c 10 port 443 and host skyroute66.com
$ sudo tcpdump -#tttt -c 10 port 443 and src skyroute66.com

<img src="/Analyze Network Traffic with TCPDump/skyroute 5.png">


$ sudo tcpdump -#tttt -c 10 443
<img src="/Analyze Network Traffic with TCPDump/shell script 3 -x  executable.png">

<img src="/Analyze Network Traffic with TCPDump/shell script 5 run.png">

<img src="Analyze Network Traffic with TCPDump/shell script 6.png">














