# Google Dork List - Uncover the Hidden Gems of the Internet ( There are at least 320+ categories ) 🌐

![Language](https://img.shields.io/badge/language-txt-orange)

Welcome to the fascinating world of Google dorks, where we unveil the secret pathways of the internet! 🚀

## 💡 What are Google Dorks?

Google dorks are specially crafted search queries that use a combination of advanced search operators to fine-tune your Google searches. By employing these dorks, you can focus on specific search results, unveiling hidden gems that ordinary searches might miss.

## 🔍 Syntax and Usage

Google dorks follow a particular syntax using advanced search operators that refine search results. Some popular operators include:

- **intitle**: Searches for pages with a specific keyword in the title.
- **inurl**: Searches for URLs containing a specific keyword.
- **filetype**: Narrows results to- `intitle`: Searches for pages with a specific keyword in the title.
- **inurl**: Searches for URLs containing a specific keyword.
- **filetype**: Narrows results to specific file types (e.g., `pdf`, `doc`, `csv`).
- **site**: Limits the search to a specific website (e.g., `site:example.com`).
- **intext**: Searches for pages with a specific keyword in the page content.
- **ext**: Limits results to files with a specific extension (e.g., `ext:php`).
 specific file types (e.g., `pdf`, `doc`, `csv`).
- **site**: Limits the search to a specific website (e.g., `site:example.com`).
- **intext**: Searches for pages with a specific keyword in the page content.
- **ext**: Limits results to files with a specific extension (e.g., `ext:php`).


## Usage

1. **Clone the Repository**: Clone this repository to your local machine to access the Google dork list.

```bash
git clone https://github.com/ishanoshada/GDorks.git
```

2. **Explore the Dorks**: The `dorks.txt` file in the repository contains a collection of Google dorks. Open the file using any text editor to view and use the dorks for your purposes.

3. **Using Google Dorks**: To use these dorks, simply copy and paste a dork of your choice into the Google search bar or use them with specialized search tools designed for Google hacking. Remember to exercise caution and ensure you are using these dorks responsibly and legally.


## 🔍 Category: Webcams - Peeking into the World

Discover live camera feeds from all over the globe! Marvel at breathtaking scenery, bustling streets, and serene sunsets. Be a virtual traveler with these dorks:

```
inurl:/view.shtml
intitle:"Live View / - AXIS"
inurl:/control/userimage.html
intitle:"Toshiba Network Camera" user login
intitle:"i-Catcher Console - Web Monitor"
...
```

## 💉 Category: SQL Injection (SQLi)

SQL Injection is a type of security vulnerability that allows attackers to manipulate a web application's database by injecting malicious SQL code into input fields or parameters. This can lead to unauthorized access, data leakage, or even complete control of the database.

```
inurl:"product.php?pid="
inurl:"category.php?id="
inurl:"news.php?id="
inurl:"gallery.php?id="
inurl:"article.php?id="
inurl:"profile.php?id="
inurl:"product-list.php?id="
inurl:"product-detail.php?id="
...
```

## 🥷 Category: Cross-Site Scripting (XSS)

Cross-Site Scripting (XSS) is a security vulnerability that allows attackers to inject malicious scripts into web pages viewed by other users. This can lead to session hijacking, cookie theft, or the execution of arbitrary code in the context of the victim's browser.

```
inurl:"search.php?q="
inurl:"results.php?q="
inurl:"gallery.php?name="
inurl:"blog.php?title="
inurl:"category.php?name="
inurl:"faq.php?question="
inurl:"feedback.php?comment="
...
```

## 🛡️ Category: Vulnerable Servers - Uncovering Weaknesses

Unearth vulnerable servers, weak points, and potential security risks. Help make the web safer by reporting any vulnerabilities you discover. Protect and educate!

```
intitle:"Test Page for the Apache Web Server on Fedora Core"
intitle:"Index of" "CentOS" "Test Page"
intitle:"Test Page for the Nginx HTTP Server"
...
```

## 🔒 Category: Sensitive Directories - Beware of Hidden Paths

Explore hidden directories, secret realms, and confidential data that accidentally made its way into public view. Tread carefully!

```
intitle:"Index of /admin"
intitle:"Index of /backup"
intitle:"Index of /config"
...
```

## 💽 Category: Database Files - Unveiling Sensitive Data

Stumble upon database files that might contain sensitive information. Handle with care and utmost respect for privacy.

```
filetype:sql intext:username password
filetype:sql "insert into" (pass|passwd|password)
...
```

## 🚪 Category: Login Pages - Enter the Gateway

Discover login portals, access points, and entryways into secured systems. Respect the sanctity of access controls and never trespass!

```
intitle:"Login" inurl:/login
intitle:"Login" inurl:/signin
...
```

## 📡 Category: Network Devices - Journey through Networking World

Navigate through network devices, routers, and access points. Find and secure, but never intrude!

```
intitle:"RouterOS" inurl:/winbox
intitle:"Ubiquiti" intext:"airOS"
...
```

## 🎥 Category: CCTV Systems - Peering through Surveillance

Explore CCTV systems, camera setups, and surveillance feeds. Respect privacy and avoid unethical use!

```
intitle:"DVR Login" inurl:/login.htm
...
```

## 🔐 Category: Apache Tomcat - Unveil Tomcat Servers

Discover Apache Tomcat servers and applications. Handle with care and report any vulnerabilities responsibly!

```
intitle:"Apache Tomcat" intext:"Apache Tomcat"
...
```

## 🛑 Category: Error Messages - Understanding Errors

Analyze various error messages to understand web server behavior and potential weaknesses. Report responsibly!

```
intext:"Error 404: Not Found"
...
```

## 🗃️ Category: Git Repository Files - Exploring Repositories

Stumble upon Git repositories, codebases, and version control systems. Respect intellectual property and never exploit!

```
filetype:gitweb inurl:git
...
```

## ⚙️ Category: Configuration Files - Delving into Settings

Uncover configuration files and system settings. Treat them with utmost care and privacy!

```
filetype:conf inurl:web.config
...
```

## 💡 Category: PHP Info Files - PHP Insights

Discover PHP information files. Handle this knowledge responsibly!

```
filetype:php inurl:info
...
```

## 📜 Category: Wordpress Sites - Enter the World of WordPress

Explore WordPress sites and blogs. Respect intellectual property and refrain from unauthorized access!

```
inurl:/wp-admin
...
```

## 📁 Category: Open Directory Listings - Directory Treasure Hunt

Embark on a quest to find open directories with valuable content. Treat what you find with respect and privacy!

```
intitle:"Index of /" + "backup"
...
```

## 🌟 Category: Google Drive Links - Drive to the Clouds

Unlock direct links to Google Drive files. Respect the owner's privacy and intellectual property!

```
inurl:"/uc?id="
...
```

## 📜 Category: Wordpress Configuration Files - WordPress Secrets

Stumble upon WordPress configuration files. Handle them responsibly and respect privacy!

```
filetype:txt inurl:wp-config
...
```

## 🔐 Category: AWS Access Keys - AWS Wonderworld

Find AWS access keys, but be cautious! Report responsibly and never exploit!

```
filetype:pem intext:PRIVATE KEY
...
```

## 🗃️ Category: Configuration Files - Hunting Configuration

Discover various configuration files. Handle with care, and never misuse!

```
filetype:env intext:AWS_SECRET_ACCESS_KEY
...
```

## Google Dork List - Contribute and Discover

Help build a comprehensive and responsible Google dork list! Contribute ethically and let's explore the internet responsibly together.


## Stargazers

[![Stargazers repo roster for @ishanoshada/GDorks](https://reporoster.com/stars/dark/ishanoshada/GDorks)](https://github.com/ishanoshada/GDorks/stargazers)
[![Forkers repo roster for @ishanoshada/GDorks](https://reporoster.com/forks/dark/ishanoshada/GDorks)](https://github.com/ishanoshada/GDorks/network/members)

> Note: This list is for educational purposes only. Always use Google dorks responsibly and never engage in any unauthorized or unethical activities. Respect privacy, intellectual property, and abide by all applicable laws and regulations. Let's make the internet a safer and more secure place! Happy dorking! 🌟
