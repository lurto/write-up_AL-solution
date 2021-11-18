
# Write-Up : AL-Solution Pentest

Write-Up for the AL-Solution TryHackMe room **(not uploaded)**

[AL-Solution room](https://github.com/lurto) 



## Recon

How many ports are open ?

```
X
```
**Use : NMAP**

What is the smb server port ?

```
445
```

What other port should you check out ?

```
80
```

## SMB

Which smb share is the most exploitable ?

```
Public
```

What is the flag ?

```
X
```
**It's a directory**

Who has a vulnerable password ? 

```
Erwan
```
**In the note**

## WordPress

What is the wordpress login password ?

```
liverpool
```
**bruteforce wordpress with rockyou.txt and the Erwann user**

What file extension will you use for a reverse shell ?

```
.php
```
**Use :** [reverse shell from pentestmonkey](https://github.com/pentestmonkey/php-reverse-shell) 

## Privilege Escalation

Where is a misconfiguration that can you use for Privilege Escalation

```
crontab
```
**the crontab executes with root a writable file**

What is the flag ?

```
X
```

## Root

What is the root flag ?

```
X
```
## Authors

- [@Burly](https://github.com/Burly0)
- [@lurto](https://www.github.com/lurto)

