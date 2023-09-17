<h3>Analyze Network Layer Communication - DNS and ICMP logs </h3>

You can inspect network traffic and network data to determine what is causing network-related issues during cybersecurity incidents. <br>

<strong>Scenario:</strong>
<p>
You are a cybersecurity analyst working at a company that specializes in providing IT consultant services. Several customers contacted your company to report that they were not able to access the company website www.yummyrecipesforme.com, and saw the error “destination port unreachable” after waiting for the page to load.

You are tasked with analyzing the situation and determining which network protocol was affected during this incident. To start, you visit the website and you also receive the error “destination port unreachable.” Next, you load your network analyzer tool, tcpdump, and load the webpage again. This time, you receive a lot of packets in your network analyzer. The analyzer shows that when you send UDP packets and receive an ICMP response returned to your host, the results contain an error message: “udp port 53 unreachable.” 
</p>


<img src="https://github.com/Nisha318/Nisha318.github.io/blob/master/assets/images/DNS%20and%20ICMP%20log.PNG">




<strong>Findings: </strong>

<img src="https://github.com/Nisha318/Nisha318.github.io/blob/master/assets/images/DNS%20and%20ICMP%20log%202.PNG">

<img src="https://github.com/Nisha318/Nisha318.github.io/blob/master/assets/images/DNS%20and%20ICMP%20log%203.PNG">


<h3> Cybersecurity Incident Report: Network Traffic Analysis</h3>

<h4>I. Summary of the Issue:</h4>
The UDP protocol reveals that the DNS server is down or unreachable.  As evident by the results of the network analysis, the ICMP echo reply returned the error message "udp port 53 unreachable".  Port 53 is commonly used for DNS protocol traffic.  It is highly likely that the DNS server is possibly in an outage state and therefore not responding.


<h4> II.  Analysis and Proposed Solution to Mitigate the Issue </h4>

The incident occurred today at 1:23 p.m.  Customers called the organization to notify the IT team that they received the message "destination port unreachable" when they attempted to visit the website.  The network security team within the organization is currently investigating the issue so customers will be able to access the website again.  In our investigation into the issue, we conducted packet sniffing tests using tcpdump.  In the resulting log file, we found that DNS port 53 was unreachable.  The next step is to identify whether the DNS server is down or traffic to port 53 is blocked by the firewall.  The DNS server might be down due to a successful Denial of Service attack or a misconfiguration.































