# Weeks 7 & 8 of CodePath Cybersecurity Write-Up 

### **Unit 7**

### Challenge 0: Install Vagrant  


Navigate to Path: 
**C:\Users\esam5\WPDistillery** on Windows 

Run ```vagrant up```

![](https://media.giphy.com/media/qaSyq5l09ei9qtphr5/giphy.gif)

----

### Challenge 1: Running WordPress with VirtualBox

Verify wpdistillery.vm is running ```ping 192.168.33.10``` 

returns:

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/challenge_1.png)

----

### Challenge 2: Kali, meet WordPress

```wget -qO- 'http://wpdistillery.vm' | gawk -v IGNORECASE=1 -v RS='</title' 'RT{gsub(/.*<title[^>]*>/,"");print;exit}'```

returns:

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/challenge_2.png)


----

### Challenge 3: WordPress Basics

Post on Wordpress Site: 

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/challenge_3.png)

### Challenge 4: Looking Under the Hood

PHP source for writing a comment:

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/challenge_4.png)

### Challenge 5: Casing the Joint

```wpscan --url http://wpdistillery.vm --random-user-agent```

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/challenge_5.png)

### Challenge 6: WordPress Time Machine

After removing the latest version of vagrant, install vagrant version 4.2:

```vagrant up```

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/challenge_6.png)

### Challenge 7: WordPress Time Machine


After running ```vagrant up``` once to provision a new VM with WP 4.2, we get new vulnerabilities 

(We choose 3-5)

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/challenge_7.png)



### **Unit 8**


### Milestone 0: Preparing the Playing Field
* Add another adapter to the virtual box Kali Machine
  * lo (loopback) with IP address of 127.0.0.1
  * eth0 (NAT) with IP similar to 10.x.x.x
  * eth1 (Host-only) with IP of 192.168.33.100 

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_0.png)

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_0_verify_connection.png)

### Milestone 1: Opening an Attack Surface

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_1_critical_security.png)


### Milestone 2: Recon

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_2_critical_security.png)


### Milestone 3: Hello, Metasploit

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_3_metasploit.png)

### Milestone 4: Pwnage 
 
Currently stuck here, antivirus interferes with metasploit shenanigans 

# Project 7 - WordPress Pentesting

Time spent: **5.5** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

### 1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 2. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 3. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 4. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
### 5. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.