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

![Screenshot_2024-03-19_23-19-31](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/5b69e523-16d5-4fcf-84fb-5a6d8ba6cccb)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![Screenshot_2024-03-19_23-20-52](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/1468b14c-636b-4130-b1ec-27ea4c7fe6ed)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot_2024-03-19_23-21-42](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/4279270a-5911-4265-a6e2-67582ca3907f)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![Screenshot_2024-03-19_23-22-42](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/70e3162a-a3f7-4521-8804-f23c0bef704a)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![Screenshot_2024-03-19_23-25-04](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/91d7e754-af6a-4fb8-a71a-862bee61615d)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![Screenshot_2024-03-19_23-25-47](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/e8bc141c-afc6-457d-9992-b713245e6ca1)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot_2024-03-19_23-26-27](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/e293a641-7556-42d4-85f7-bd20481f9588)


 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot_2024-03-19_23-29-40](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/aad0b7f5-9275-4eb0-ac52-584fc0e2eb24)

![Screenshot_2024-03-19_23-31-17](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/0ea3b400-1b39-494c-a4d9-8c45dfa6e485)


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

![Screenshot_2024-03-19_23-32-49](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/f5974d1f-c22d-41cc-9c11-11ea5c8f1052)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


![Screenshot_2024-03-19_23-34-42](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/c90be246-d3d5-4d68-858d-1bb7227fbbc3)

![Screenshot_2024-03-19_23-35-55](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/55e52146-7db5-4fa5-bdaf-86ec8b988a8d)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
![Screenshot_2024-03-19_23-41-33](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/a96122cb-a846-4010-a795-ef7047f0f590)

 
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot_2024-03-19_23-43-21](https://github.com/MaheshS03/EH-Enumeration/assets/128498431/f3fd91ad-101d-4e25-a65b-71439c9b5aaf)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

