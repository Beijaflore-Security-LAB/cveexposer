#### DESCRIPTION
This Script search in cve.circl.lu known CVE & Exploit to qualified them with the following rules :

       Critical when CVSS >= 9 
       High when CVSS < 9 & >= 7 
       Medium when CVSS <= 4 & > 7 
       Low when CVSS < 4 


#### GUIDE 
To launch the script :

```sh
 cveexposer -p <product> -v <version>
   -h : help
   -p : for the product
   -v : for version because fuck verbose
```
   
Examples :
```sh
   cveexposer -p nginx -v 1.3.10
   cveexposer -p drupal -v 7
```
