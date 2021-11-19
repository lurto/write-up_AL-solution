
# Write-Up : AL-Solution Pentest

Write-Up for the AL-Solution TryHackMe room **(not uploaded)**

[AL-Solution room](https://github.com/lurto) 



## Recon

How many ports are open ?

```
4
```
**Use : NMAP**

What is the smb server port ?

```
445
```

What is the other port the you need to check ?

```
80
```

## Exploiting SMB

Which smb share is the most exploitable ?

```
PublicShare
```

Who has a vulnerable password ? 

```
Erwan
```
**In the note**

## Exploiting WordPress

What is the version of the wordpress

```
5.8.2
```

What is the wordpress login password ?

```
liverpool
```
**bruteforce wordpress with rockyou.txt and the erwan user**

## Getting a reverse shell

In order to gain acces on the machines we need to execute code on the machine. Lucky us, we can edit files in the wordpress. You need to change the php code on one of the files and call this page to execute the reverse shell
![image](https://user-images.githubusercontent.com/90036439/142603796-67e404fb-5b53-436c-84f7-23fb5ffd77f7.png)






What file extension will you use for a reverse shell ?

```
.php
```
**Use :** [reverse shell from pentestmonkey](https://github.com/pentestmonkey/php-reverse-shell) 

What is the user you get after getting the reverse shell 

```
www-data
```

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

