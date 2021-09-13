---
published: true
---
## further nmap

<dl>
  <dt>Task 1</dt>
  <dd>why nmap? The short answer is that it's currently the industry standard for a reason: no other port scanning tool comes close to matching its functionality </dd>
   
  <dt>Task 2 </dt>
  <dd>Nmap can be accessed by typing nmap into the terminal command line, followed by some of the switches 
  </dd>

 
  
   <dt>Task 3</dt>
  <dd> When port scanning with Nmap, there are three basic scan types. These are:

TCP Connect Scans (-sT)
SYN "Half-open" Scans (-sS)
UDP Scans (-sU)Which RFC defines the appropriate behaviour for the TCP protocol?

    RFC 793
If a port is closed, which flag should the server send back to indicate this?

Correct Answer: rst


</dd>

   <dt>Task 4</dt>
  <dd> 
As with TCP scans, SYN scans (-sS) are used to scan the TCP port-range of a target or targets; however, the two scan types work slightly differently. SYN scans are sometimes referred to as "Half-open" scans, or "Stealth" scans.

</dd>
  
   <dt>Task 5</dt>
  <dd> When a packet is sent to an open UDP port, there should be no response. When this happens, Nmap refers to the port as being open|filtered. 
  

</dd>
  <dt>Task 6</dt>
  <dd> NULL, FIN and Xmas TCP port scans are less commonly used than any of the others we've covered already, so we will not go into a huge amount of depth here. All three are interlinked and are used primarily as they tend to be even stealthier, relatively speaking, than a SYN "stealth" scan. 


</dd>
   <dd> 
     Which of the three shown scan types uses the URG flag?

Correct Answer: xmas
Why are NULL, FIN and Xmas scans generally used?

Correct Answer: firewall evasion
Which common OS may respond to a NULL, FIN or Xmas scan with a RST for every port?

Correct Answer: microsoft windows

  

</dd>
 <dt>Task 7</dt>
  <dd> To perform a ping sweep, we use the -sn switch in conjunction with IP ranges which can be specified with either a hypen (-) or CIDR notation. i.e. we could scan the 192.168.0.x network using:

nmap -sn 192.168.0.1-254
or

nmap -sn 192.168.0.0/24

</dd>
  
  <dt>Task 8</dt>
  <dd> safe:- Won't affect the target
intrusive:- Not safe: likely to affect the target
vuln:- Scan for vulnerabilities
exploit:- Attempt to exploit a vulnerability
auth:- Attempt to bypass authentication for running services (e.g. Log into an FTP server anonymously)
brute:- Attempt to bruteforce credentials for running services
discovery:- Attempt to query running services for further information about the network (e.g. query an SNMP server).
  </dd>
  
   <dt>Task 9</dt>
  <dd> What optional argument can the ftp-anon.nse script take?

Correct Answer: maxlist

  

</dd>
  
  <dt>Task 10</dt>
  <dd> Search for "smb" scripts in the /usr/share/nmap/scripts/ directory using either of the demonstrated methods. 
What is the filename of the script which determines the underlying OS of the SMB server?

Correct Answer: smb-os-discovery.nse
Read through this script. What does it depend on?

Correct Answer: smb-brute



</dd>
  
  <dt>Task 11</dt>
  <dd> Which simple (and frequently relied upon) protocol is often blocked, requiring the use of the -Pn switch?

Correct Answer: icmp
[Research] Which Nmap switch allows you to append an arbitrary length of random data to the end of packets?

Correct Answer: -data-length 
    </dd>
  
    

  
</dl>
