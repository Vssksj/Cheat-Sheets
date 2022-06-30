# Wonderful Cheat-Sheet for *Nmap*

## Introduction

Nmap is a famous open-source scanner created by *Gordon Lyon*. This is a tool used to discover services and hosts on a network. To install it, a simple `apt install nmap`.



## Commands 

Nmap has many options : **Scanning** TCP/UDP ports, **discovering** hosts, **collecting** versions of services, ...

Let's start with **basic scan** options !

INFO : All commands are detailled in the man page (`man nmap`).

# Scan
- Simple scan on a specific IP Adress, the most basic :
  ```
  nmap 10.10.14.19
  ```
- Scan all the ports 
  ````
  nmap -p- 10.10.14.19
  ````
- Scan UPD ports
  ````
  nmap -sU 10.10.14.19
  ````
- Scan versions of open services
  ````
  nmap -sV 10.10.14.19
  ````

# Useful options

This is most used commands and the most useful :

- `-Pn` : Skip 
- `-T1/5` : + or - scan ( Fast or not )
- `-A` = `-sC` + `-sV` : Version + default nmap script 
- `-oN/G/A` : Output format
- `-p-` : Scan all ports


# You can combine switch to do your scan faster.


## Examples

Imagine your a pentester and you need to scan the IP Adress `10.10.14.20` :

You are going to make some scans : 

- First, you can make a scan to know all open ports :
  ````
  nmap -p- 10.10.14.20
  ````
- Now, you can precise open ports, collect versions and write in a output file the result :
  ````
  nmap -p22,80,1337 10.10.14.20 -A -oN output_nmap.txt
  ````

# Conclusion

Now, you know the basic commands of *Nmap* and you can start to use its to train yourself on [TryHackMe](https://tryhackme.com), [HackTheBox](https://app.hackthebox.com) or [Vulnhub](https://vulnhub.com).
