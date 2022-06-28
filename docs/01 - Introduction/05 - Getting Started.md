# Getting started

- Stay organized

- Note taking tools:
	- [Cherrytree](https://www.giuspen.com/cherrytree)
	- [Visual Studio Code](https://code.visualstudio.com)
	- [Evernote](https://evernote.com)
	- [Sublime Text](https://www.sublimetext.com)
	- [GitBook](https://www.gitbook.com)
	- [Notion](https://www.notion.so)
	- [Notepad++](https://notepad-plus-plus.org/downloads)





---

<details>
  <summary>T001</summary>
  
  ```
	 Target: 10.129.62.97

	1. Perform an Nmap scan of the target. What is the version of the service that is running on port 8080?
		- Apache Tomcat

	2. Perform an Nmap scan of the target and identify the non-default port that the telnet service running on.
		- 2323

	3. List the SMB shares available on the target host. Connect to the available share as the bob user. Once connected, access the folder called 'flag' and submit the contents of the flag.txt file.
		- dceece590f3284c3866305eb2473d099
  ```

</details>


<details>
  <summary>S001</summary>
  
  ```bash
	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ nmap -sC -sV -p- 10.129.160.49 -oN 1.txt
	Starting Nmap 7.92 ( https://nmap.org ) at 2022-06-28 21:38 CEST
	...
	...
	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ cat 1.txt | grep 8080
	8080/tcp open  http        Apache Tomcat

	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ cat 1.txt | grep telnet
	2323/tcp open  telnet      Linux telnetd

	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$  smbclient -U bob \\\\10.129.62.104\\users
	Password for [WORKGROUP\bob]:
	Try "help" to get a list of possible commands.
	smb: \> ls
	  .                                   D        0  Fri Feb 26 00:06:52 2021
	  ..                                  D        0  Thu Feb 25 21:05:31 2021
	  flag                                D        0  Fri Feb 26 00:09:26 2021
	  bob                                 D        0  Thu Feb 25 22:42:23 2021

			4062912 blocks of size 1024. 944784 blocks available
	smb: \> cd flag
	smb: \flag\> ls
	  .                                   D        0  Fri Feb 26 00:09:26 2021
	  ..                                  D        0  Fri Feb 26 00:06:52 2021
	  flag.txt                            N       33  Fri Feb 26 00:09:26 2021

			4062912 blocks of size 1024. 944784 blocks available
	smb: \flag\> get flag.txt
	getting file \flag\flag.txt of size 33 as flag.txt (0.2 KiloBytes/sec) (average 0.2 KiloBytes/sec)
	smb: \flag\> exit

	┌──(x0r㉿kreatur-der-nacht)-[~]
	└─$ cat flag.txt           
	dceece590f3284c3866305eb2473d099
    }
  ```
</details>

---