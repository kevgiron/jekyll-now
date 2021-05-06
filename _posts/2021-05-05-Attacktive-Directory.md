---
published: false
---
## Attacktive-Directory

<dl>
  <dt>Task 1</dt>
  <dd>Deploy The Machine</dd>
 
  <dd>Once connected to the VPN, deploy the machine</dd>
  

  <dt>Task 2</dt>
  <dd> What tool will allow us to enumerate port 139/445?</dd>
 
  <dd>enum4linux</dd>
  <dd>What is the NetBIOS-Domain Name of the machine?
 </dd>
 
  <dd> THM-AD</dd>

  <dt>Task 3</dt>
  <dd>What invalid TLD do people commonly use for their Active Directory Domain?</dd>
 
  <dd>.local</dd>

  
  <dt>Task 4</dt>
  
  <dd>Enumerating Users via Kerberos</dd>

  <dd>What command within Kerbrute will allow us to enumerate valid usernames?</dd>
 
  <dd>userenum</dd>
  dd>What notable account is discovered?</dd>
 
  <dd>svc-admin</dd>
  
 <dt>Task 5</dt>
 
 <dd>We have two user accounts that we could potentially query a ticket from. Which user account can you query a ticket from with no password?</dd>
 
  <dd>svc-admin</dd>
 
  <dd>what type of Kerberos hash did we retrieve from the KDC? </dd>

  <dd>Kerberos 5 AS-REP etype 23</dd>
  <dd>What mode is the hash?</dd>
  

  <dd>18200</dd>
 
  <dd>Now crack the hash with the modified password list provided, what is the user accounts password?
</dd>

  <dd>management2005</dd>
  
 
  
  <dt>Task 6</dt>
  <dd>With a user's account credentials we now have significantly more access within the domain. We can now attempt to enumerate any shares that the domain controller may be giving out.</dd>
 
  <dd>Using utility can we map remote SMB shares?
</dd>

  <dd>smbclient</dd>
  
  
 
  <dd>How many remote shares is the server listing?</dd>

  <dd>6</dd>
  <dd>What is the content of the file?</dd>
  <dd>YmFja3VwQHNwb29reXNlYy5sb2NhbDpiYWNrdXAyNTE3ODYw</dd>
 
  <dd>Decoding the contents of the file, what is the full contents?
</dd>

  <dd>backup@spookysec.local:backup2517860</dd>
  
  <dt>Task 7</dt>
  <dd>What method allowed us to dump NTDS.DIT?</dd>
 
  <dd>DRSUAPI</dd>

  <dd>What is the Administrators NTLM hash?
</dd>

<dd>0e0363213e37b94221497260b0bcb4fc</dd>
 
  <dd>What method of attack could allow us to authenticate as the user without the password?</dd>
 
  <dd>pass the hash</dd>

  <dd>Using a tool called Evil-WinRM what option will allow us to use a hash?</dd>

   <dd>H</dd>
 
 
 <dt>Task 8</dt>
  <dd>Flag Submission Panel</dd>
 
  <dd>svc-admin: TryHackMe{K3rb3r0s_Pr3_4uth}</dd>

  <dd>backup:TryHackMe{B4ckM3UpSc0tty!}
</dd>

<dd>administrator:TryHackMe{4ctiveD1rectoryM4st3r}</dd>
 
</dl>


