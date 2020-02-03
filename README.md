#### DESCRIPTION
This Script searches in cve.circl.lu known CVE & Exploit and qualify them with the following rules :

       Critical when CVSS >= 9 
       High when CVSS < 9 & >= 7 
       Medium when CVSS <= 4 & > 7 
       Low when CVSS < 4 

This script uses jq and bc.

#### GUIDE 
To launch the script :

```
 cveexposer -p <product> -v <version>

   -h : help
   -p : for the product
   -v : for version because fuck verbose
 ```
   
Examples :
```console
foo@bar:~$ cveexposer -p nginx -v 1.3.10
Detect 6 CVE for nginx 1.3.10 : [0 critical,3 high,3 medium,0 low]
```
```console
foo@bar:~$ cveexposer -p drupal -v 8
Detect 18 CVE for drupal 8 : [0 critical,2 high,16 medium,0 low] and 3 public exploits [CVE-2018-7600 CVE-2018-7600 CVE-2018-7600]
```
