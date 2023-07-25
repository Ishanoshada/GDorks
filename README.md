# Google Dork List

This repository contains a collection of Google dorks categorized by topics. Google dorks are specialized search queries that leverage Google's advanced search operators to find specific information on the internet. They can be useful for cybersecurity professionals, penetration testers, or anyone interested in exploring potential vulnerabilities or sensitive information exposed on the web.

## Usage

1. **Clone the Repository**: Clone this repository to your local machine to access the Google dork list.

```bash
git clone https://github.com/ishanoshada/GDorks.git
```

2. **Explore the Dorks**: The `dorks.txt` file in the repository contains a collection of Google dorks sorted by categories. Open the file using any text editor to view and use the dorks for your purposes.

3. **Using Google Dorks**: To use these dorks, simply copy and paste a dork of your choice into the Google search bar or use them with specialized search tools designed for Google hacking. Remember to exercise caution and ensure you are using these dorks responsibly and legally.

## Categories

### Website Vulnerabilities

1. `intitle:"Test Page for Apache Server"` - Finds test pages for Apache servers.
2. `intitle:"Welcome to nginx!" intext:"Welcome to nginx on Debian!"` - Reveals websites using nginx on Debian.
3. `inurl:"/wp-admin/" intitle:"WordPress Administrator Login"` - Finds WordPress administrator login pages.

### Sensitive Directories

4. `intitle:"Index of /" "Parent Directory"` - Lists directories with open listing.
5. `intitle:"Index of /admin"` - Explores websites with "admin" directories exposed.

### Database Exposed

6. `intext:"Welcome to phpMyAdmin"` - Discovers websites using phpMyAdmin.
7. `intext:"phpMyAdmin MySQL-Dump"` - Unveils MySQL dump files.

### Network Devices

8. `intitle:"RouterOS" inurl:"winbox"` - Discovers MikroTik RouterOS Winbox.
9. `intitle:"Ubiquiti AirOS"` - Reveals Ubiquiti AirOS devices.

### File Types

10. `filetype:pdf "confidential"` - Finds PDF files containing the term "confidential."
11. `filetype:log "PHP Error" -"admin"` - Discovers log files with PHP errors, excluding admin references.

### Private Information

12. `intext:"@gmail.com" filetype:txt` - Discovers text files containing Gmail addresses.
13. `intext:"username" intext:"password" filetype:txt` - Reveals text files containing login credentials.

## Disclaimer

Using Google dorks to access sensitive or unauthorized information is illegal and unethical. This repository is intended for educational purposes only. Do not use these dorks to engage in any unauthorized activities or violate anyone's privacy.

## Contribution

Contributions to this Google Dork List are welcome! If you know of other useful and responsible dorks, feel free to submit a pull request to enhance the list.

Stay ethical, stay secure! Happy dorking!

---

The `dorks.txt` file:

```
intitle:"Test Page for Apache Server"
intitle:"Welcome to nginx!" intext:"Welcome to nginx on Debian!"
inurl:"/wp-admin/" intitle:"WordPress Administrator Login"
intitle:"Index of /" "Parent Directory"
intitle:"Index of /admin"
intext:"Welcome to phpMyAdmin"
intext:"phpMyAdmin MySQL-Dump"
intitle:"RouterOS" inurl:"winbox"
intitle:"Ubiquiti AirOS"
filetype:pdf "confidential"
filetype:log "PHP Error" -"admin"
intext:"@gmail.com" filetype:txt
intext:"username" intext:"password" filetype:txt
```

