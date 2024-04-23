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

![1](https://github.com/Gopikakarthik/Enumeration/assets/121235427/2ff48f09-8f88-4211-9890-585c22be179a)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![2](https://github.com/Gopikakarthik/Enumeration/assets/121235427/342ad6fb-d51d-480e-a09b-cf380826001a)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![3](https://github.com/Gopikakarthik/Enumeration/assets/121235427/c129f8a8-b7d7-41fc-9d28-26295f27b97d)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![4](https://github.com/Gopikakarthik/Enumeration/assets/121235427/5f1477b1-d362-475c-9112-900aaf2d5410)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![5](https://github.com/Gopikakarthik/Enumeration/assets/121235427/02bd4394-c5d4-4cf7-ba29-6afb3425b682)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![6](https://github.com/Gopikakarthik/Enumeration/assets/121235427/f0222fd1-ae8e-4640-88a4-e454cff88727)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![7](https://github.com/Gopikakarthik/Enumeration/assets/121235427/35116949-69e2-414f-8b02-c972d43039fc)

#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![8](https://github.com/Gopikakarthik/Enumeration/assets/121235427/68291e51-f9ae-482c-bcbe-42cddd85efb2)


##dnsenum
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

![9](https://github.com/Gopikakarthik/Enumeration/assets/121235427/668988b1-8df7-4ffc-a31f-83cc03e4be28)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![10](https://github.com/Gopikakarthik/Enumeration/assets/121235427/769b7a95-3c7a-49a5-9b3f-3784fb358048)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![11](https://github.com/Gopikakarthik/Enumeration/assets/121235427/5f564e93-3043-4116-b8fd-b1bf5ae10fa9)

select any username in the first column of the above file and check the same
![12](https://github.com/Gopikakarthik/Enumeration/assets/121235427/4aac4b06-7ad7-4c3e-afe2-784dc4e643a9)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
 ![13](https://github.com/Gopikakarthik/Enumeration/assets/121235427/0783f5d2-1b57-4e42-93f1-bdd5b5c43c5b)


  
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![14](https://github.com/Gopikakarthik/Enumeration/assets/121235427/903079f2-6c90-4aee-b637-aeef27a55bc9)




## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

