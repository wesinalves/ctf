# Linux room from tryhackme.com

## what was done
privilege escalation technique

```sh
shiba1 -> shiba2 -> shiba3 -> shiba4 -> shiba3 -> nootnoot
```

## what was learnt

searching for vulnerabilities using [linpeas.sh][linpeas]

create a http server using ```python -m http.server```

redirect error logs using ```2> /dev/null``` combined with *find* command

```less -r file``` to see large files

```command | tee file``` sends output to terminal and a file as well

## tools 
[linpeas.sh][linpeas]

wget

http.server

[linpeas]: https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/linPEAS
