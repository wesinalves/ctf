# Vulnversity room

This room breaks each OWASP topic down and includes details on what the vulnerability is, how it occurs and how you can exploit it. You will put the theory into practise by completing supporting challenges.

## what was done

* Injection
* Broken Authentication
* Sensitive Data Exposure
* XML External Entity
* Broken Access Control
* Security Misconfiguration
* Cross-site Scripting
* Insecure Deserialization
* Components with Known Vulnerabilities
* Insufficent Logging & Monitoring

## what was learnt

re-registration attack
sqllite db
look at repositories in github to find misconfiguration application and servers

### Crossite script

[http://www.xss-payloads.com/]

**Payloads**
```
<script>alert(window.location.hostname)</script>
<b>Coding Rocks</b>
<script>alert(document.cookie)</script>
<script>document.querySelector('#thm-title').textContent = 'I am a hacker'</script>
```

### Deserialization

decode a base64 string: ```echo some string | base64 -d```

## tools

