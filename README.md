# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:
To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:
Install kali linux either in partition or virtual box or in live mode

### Step 2:
Investigate on the various Google hacking keywords and enumeration tools as follows:

### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:



site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
### output
<img width="1052" height="500" alt="1" src="https://github.com/user-attachments/assets/b82d294a-59d3-4a8a-a20f-49d2558495c8" />




filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
### output
<img width="1045" height="503" alt="2" src="https://github.com/user-attachments/assets/2c35b0e7-5398-41aa-8d8c-49fd0bae9783" />



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
### output
<img width="1052" height="507" alt="3" src="https://github.com/user-attachments/assets/32839553-7205-4802-a404-88a897410750" />



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
### output
<img width="1042" height="502" alt="4" src="https://github.com/user-attachments/assets/0adfe9d7-4da5-423e-b0c3-5d5baef7a706" />



intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
### output
<img width="1043" height="505" alt="5" src="https://github.com/user-attachments/assets/92cb132a-87c6-4dd2-b2bb-d1bf2aeb8f77" />



link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
### output
<img width="1045" height="505" alt="6" src="https://github.com/user-attachments/assets/a6f4ea39-2be1-4c82-b1a7-87cd3fd6de2e" />



cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
### output
<img width="1024" height="571" alt="7" src="https://github.com/user-attachments/assets/47754c25-058d-4d2c-8a93-bbe2156440a5" />

<img width="1024" height="367" alt="8" src="https://github.com/user-attachments/assets/52839131-b575-41e8-b81a-1a023012e6d2" />



## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
### output
<img width="1024" height="430" alt="9" src="https://github.com/user-attachments/assets/4e2a623b-e464-4540-b4ed-45c6072db4db" />

<img width="1024" height="506" alt="10" src="https://github.com/user-attachments/assets/b6daf519-7541-497a-8ab8-664dc151afb3" />



## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same
## output
<img width="840" height="223" alt="image" src="https://github.com/user-attachments/assets/5c2f31ce-e517-4d40-b944-f9a4c11eae9c" />
<img width="1024" height="539" alt="12" src="https://github.com/user-attachments/assets/be1d8f84-f575-4e4d-8db3-dde6ca7eca8f" />



## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
### output
<img width="1024" height="446" alt="13" src="https://github.com/user-attachments/assets/d65ba89b-1b22-44cf-9d57-f4d50267a684" />

  

## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
### output
<img width="1024" height="280" alt="14" src="https://github.com/user-attachments/assets/eb9dcfec-c69d-4aee-ae08-83bd6c8c3de6" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

