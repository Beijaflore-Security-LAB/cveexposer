#### DESCRIPTION
This Script search in cve.circl.lu known CVE & Exploit to qualified them with the following rules :

       Critical when CVSS >= 9 
       High when CVSS < 9 & >= 7 
       Medium when CVSS <= 4 & > 7 
       Low when CVSS < 4 


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
