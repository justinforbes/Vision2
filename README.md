# Vision

Nmap's XML result parse and NVD's CPE correlation to search CVE. You can use that to find public vulnerabilities in services... 

```..::: VISION v0.1 :::...
Nmap\'s XML result parser and NVD's CPE correlation to search CVE

Example:
python vision2.py -f result_scan.xml -l 3 -o txt

Coded by Mthbernades and CoolerVoid

- https://github.com/mthbernardes
- https://github.com/CoolerVoid

usage: vision2.py [-h] -f NMAPFILE [-l LIMIT] [-o OUTPUT]
vision2.py: error: argument -f/--nmap-file is required

```

## Example of results:
```
$ python Vision-cpe.py -f result_scan.xml -l 3 -o txt

::::: Vision v0.1 - nmap NVD's cpe correlation - Coded by CoolerVoid
Host: 127.0.0.1
Port: 53
cpe:/a:isc:bind:9.8.1:p1

	URL: https://nvd.nist.gov/vuln/detail/CVE-2016-9131
	Description: named in ISC BIND 9.x before 9.9.9-P5, 9.10.x before 9.10.4-P5, and 9.11.x before 9.11.0-P2 allows remote attackers to cause a denial of service (assertion failure and daemon exit) via a malformed response to an RTYPE ANY query.

	URL: https://nvd.nist.gov/vuln/detail/CVE-2016-8864
	Description: named in ISC BIND 9.x before 9.9.9-P4, 9.10.x before 9.10.4-P4, and 9.11.x before 9.11.0-P1 allows remote attackers to cause a denial of service (assertion failure and daemon exit) via a DNAME record in the answer section of a response to a recursive query, related to db.c and resolver.c.

	URL: https://nvd.nist.gov/vuln/detail/CVE-2016-2848
	Description: ISC BIND 9.1.0 through 9.8.4-P2 and 9.9.0 through 9.9.2-P2 allows remote attackers to cause a denial of service (assertion failure and daemon exit) via malformed options data in an OPT resource record.
...

```

## Common questions:

## How to write XML output on Nmap ?
https://nmap.org/book/output-formats-xml-output.html

## What is a CPE  ?

https://nmap.org/book/output-formats-cpe.html

https://nvd.nist.gov/products/cpe

## What is a CVE ?

https://cve.mitre.org/


## This is a true vulnerability scanner ?

Nop, this script is util to audit banners of services, this tool don't test inputs... Vulnerability scanner its complex, look that following http://www.openvas.org/




## Authors: 

# mthbernades and CoolerVoid 

https://github.com/mthbernardes

https://github.com/CoolerVoid

Old version using SAX style parse:
https://github.com/CoolerVoid/Vision

Date: Ter Set  5 02:00:09 2017


