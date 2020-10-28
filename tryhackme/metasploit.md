# Metasploit room

Learn to use Metasploit, a tool to probe and exploit vulnerabilities on networks and servers.

## what was done

Metasploit is a set of tools to exploit a remote machine. Matasploit uses postgre to store information collected from the victim.
So, first thing to do is init the dataset using `msfdb init`.
Once dataset start, you can run `msfconsole` to exploit a machine.
You need set some variables before to start exploit.
* `set RHOSTS`
* `set LHOST`
then select the exploit using command `use name_exploit`.
Run the exploit via either command `exploit` or `run -j`

## what was learnt

modules:

* exploit
* payload
* encoder
* nop
* auxiliary
* post

Libraries:

* Rex
* MSF Core
* MSF Base

Interfaces:

* console
* cli
* gui
* rpc


## tools

icecast
'?' show help
getprivs
upload