---
published: true
---
## Metasploit

<dl>
  <dt>Task 1</dt>
  <dd>Before starting Metasploit, we can view some of the advanced options we can trigger for starting the console. Check these out now by using the command: msfconsole -h</dd>
  <dd> We can start the Metasploit console on the command line without showing the banner or any startup information as well. What switch do we add to msfconsole to start it without showing this information? This will include the '-'</dd>

  <dd>Once the database is initialized, go ahead and start Metasploit via the command: msfconsole</dd>
  <dd> After Metasploit has started, let's go ahead and check that we've connected to the database. Do this now with the command: db_status </dd>
  

  <dt>Task 3 - Escalate privileges, learn how to upgrade shells in metasploit.</dt>
  <dd> Let's go ahead and start exploring the help menu. On the Metasploit prompt (where we'll be at after we start Metasploit using msfconsole), type the command: help</dd>
 
  <dd>
Finding various modules we have at our disposal within Metasploit is one of the most common commands we will leverage in the framework. What is the base command we use for searching?
</dd>
  <dd>Metasploit has a built-in netcat-like function where we can make a quick connection with a host simply to verify that we can 'talk' to it. What command is this?

 </dd>
 
  <dd>When performing a penetration test it's quite common to record your screen either for further review or for providing evidence of any actions taken. This is often coupled with the collection of console output to a file as it can be incredibly useful to grep for different pieces of information output to the screen. What command can we use to set our console output to save to a file?</dd>
  

  <dd> Leaving a Metasploit console running isn't always convenient and it can be helpful to have all of our previously set values load when starting up Metasploit. What command can we use to store the settings/active datastores from Metasploit to a settings file? This will save within your msf4 (or msf5) directory and can be undone easily by simply removing the created settings file. 
</dd>
 <dd>Metasploit consists of six core modules that make up the bulk of the tools you will utilize within it. Let's take a quick look through the various modules, their purposes, and some of the commands associated with modules. </dd>
    <dd> Now that we've scanned our victim system, let's try connecting to it with a Metasploit payload. First, we'll have to search for the target payload. In Metasploit 5 (the most recent version at the time of writing) you can simply type use followed by a unique string found within only the target exploit. For example, try this out now with the following command use icecast. What is the full path for our exploit that now appears on the msfconsole prompt? *This will include the exploit section at the start
</dd>
 <dd>Now that we've got a shell into our victim machine, let's take a look at several post-exploitation modules actions we can leverage! Most of the questions in the following section can be answered by using the Meterpreter help menu which can be accessed through the 'help' command. This menu dynamically expands as we load more modules.

  </dd>
  </dl>
