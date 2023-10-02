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

## Output:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/87ff5a3a-9978-47d0-b54c-6514a242235c)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/fab9dd0b-a155-44fa-8764-9283f0e7ac37)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## Output:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/810b1431-9a98-4731-9ea8-dd20930f0739)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## Output:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/eac4291b-6adc-4a38-a1a8-eccb0e249539)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## Output:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/f170463f-53c5-49c5-a27f-03c0d31db853)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## Output:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/1b50e7cf-5486-4508-a63e-0e96aa56bf23)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## Output:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/ce61d6ce-7e37-498f-8ad3-6c4e6322e453)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/b2f1fe59-b5a0-4829-9fca-401cd4428116)

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
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/8755c4e3-c461-43a5-8904-7097c6115ecb)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/eae73231-3043-41c5-880e-66d1a3284085)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/83e1553d-ee63-4f76-8422-a84c2e9ac9a6)


select any username in the first column of the above file and check the same
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/900b15bc-0485-4fff-8367-bcfe6e3f831b)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
 ![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/9b7b37fc-e6d3-402e-8af4-df4714861d04)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![image](https://github.com/Prasanth9025/Enumeration/assets/118343686/ed4a1c91-7c0e-4d8c-8e3c-594167383d4c)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

