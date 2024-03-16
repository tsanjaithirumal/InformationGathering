# To perform information gathering techniques

## AIM:

To perform information gathering techniques using kali linux 

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:
Open terminal/browser and try execute necessary commands/use url to perform information gathering
## Pen Test Tools Categories:
Following Categories of pen test tools are identified for information gathering:

Footprinting is a part of the reconnaissance process which is used for gathering possible information about a target computer system or network.

http://www.whois.com/whois website to get detailed information about a domain name information including its owner, its registrar, date of registration, expiry, name server, owner's contact information, etc.
## OUTPUT:
![eth2 1](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/03c9de39-715f-4544-914f-a8dc81b7af08)

## Finding IP address:
ping command is available on Windows as well as on Linux OS. Following is the example to find out the IP address of saveetha.ac.in.

```
ping saveetha.ac.in
```
## Output:
![eth2 2](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/bf690154-8daf-4f61-b28b-c14d218fde32)


## Finding Hosting Company
```
get further detail by using ip2location.com website.
```

## Output:
![eth2 3](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/a609f01c-7774-467d-9fb1-7b27fd131df3)


## History of the website:
## Output:
https://web.archive.org/
![eth2 4](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/9944d113-4c67-47ee-a07c-2d23d30c16b6)

## Webserver Fingerprinting:
### Netcat:
```
nc 172.17.52.118 80
```
## Output:

![eth2 5](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/ddb8f37a-c510-41d3-8e56-d06e1dfbdf03)

## nmap:
```
nmap -p 21 -sV --script=banner ftp.vim.org
```
## Output:
![eth2 6](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/ae6c16e5-c427-42fc-aad4-d7a6b7139843)


### Whatweb:
```
whatweb infosys.com
```
```
whatweb zoho.com
```
```
whatweb -v -a 3 172.17.52.201
```
### Output:
![eth2 7](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/c966fc93-52b2-4567-84d8-db493e80bd8e)
![eth2 8](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/bd11482a-c1f8-4e84-8aff-dbd63e2a048a)




## httprint:
```
httprint -h 172.17.52.201 -s /usr/share/httprint/signatures.txt -P0 |more
```
### Output:

![eth2 9](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/b7e7f96c-b475-4868-8c6b-46303b8871b1)

## Tracing the Location
### TCP Traceroute:
```
sudo traceroute -T www.saveetha.ac.in
```
## Output:
![eth2 10](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/449f9bc4-1e0e-440d-8383-f4581e79874e)


## UDP Traceroute:
```
sudo traceroute -U www.saveetha.ac.in
```
## Output:
![eth 2 11](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/9af636da-8d1c-41e3-be72-598e57a10e57)


## ICMP Traceroute:
```
sudo traceroute  www.saveetha.ac.in
```
## Output:
![eth2 12](https://github.com/Rajeshanbu/InformationGathering/assets/118924713/98f95c5e-46c9-4e03-a395-1d7901d03f74)

## RESULT:
The information gathering techniques tools/procedure were identified successfully
