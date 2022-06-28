# f1r57_h4ck

Target: 157.245.46.136:32508

![[Pasted image 20220629000057.png]]

Try to identify the services running on the server above, and then try to search to find public exploits to exploit them. Once you do, try to get the content of the '/flag.txt' file. (note: the web server may take a few seconds to start)
`HTB{my_f1r57_h4ck}`

---

```bash
┌──(x0r㉿kreatur-der-nacht)-[~/jpt]
└─$ searchsploit Simple Backup                            
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- ---------------------------------
 Exploit Title                                                                                                                                                                                             |  Path
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- ---------------------------------
WordPress Plugin Simple Backup 2.7.11 - Multiple Vulnerabilities                                                                                                                                           | php/webapps/39883.txt
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- ---------------------------------
Shellcodes: No Results
```
[WordPress Plugin Simple Backup 2.7.11](https://www.exploit-db.com/exploits/39883)

![[Pasted image 20220629002008.png]]