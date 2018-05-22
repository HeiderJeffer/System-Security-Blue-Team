# eco
# System Security - Blue Team (Building a site)

* Project Coursework (Milestone 1)
* Prepared by
* Heider Jeffer hjeffer@unibz.it 
* Opaniyi Ayokunmi Tolulope ayokunmi12@gmail.com 


# PART 1

* Bolzano Souvenir Shop
Our shop called as Ayo, sell original souvenirs from Bolzano, e.g., key rings, toys, and  wallpapers.
# Requirements
* Google Drive (https://www.google.com/drive/ )
* NinjaMock (https://ninjamock.com/ )
* Java (https://java.com )
* MySQL (https://www.mysql.com/ )

# Feature 1 - User data management

* User can register with name, address, login info, etc.

# Feature 2 - List of items
Display list of item (fixed list of items).

# Feature 3 - Shopping carts 
Offering basic transactions with add to cart and buy items.

# Feature 4 - Login/logout and session management
* Login

* Logout


# PART 2
* Code injection (SQL or other).
* How to address: Use scanners and fuzzers to address injection flaws.
* How to prevent: Use Object-relational mapping (ORM) to avoid injection flaws. The following is a simple example, written in C# code, to execute a query written in SQL using a database engine.
 
In contrast, the following makes use of an ORM, allowing the writing of code which naturally makes use of the features of the language.

* Cross-site scripting (javascript or other)
* How to address: Use tools that can find some XSS problems automatically, particularly in mature technologies such as J2EE/JSP.
* How to prevent: Use framework that automatically escape XSS by design such as Spring MVC.
Misconfiguration issues (default admin accounts, etc.)
* How to address: Use automated scanners for detecting misconfigurations and use of default accounts or configurations.
* How to prevent: Use automated generation of credential information and send directly to users/admins.
Exposure of sensitive data (e.g. passwords stored in cleartext)
* How to address: By not using encryption for sensitive data or use weak encryption key.
* How to prevent: Password is encrypted in transit with secure protocols such as TLS, secured authentication of gateways in the network, conducting of  regular risk assessment on the network, keeping a protected and secure backup of the sensitive data can help to reduce these losses.
# Session management (mishandling of session ids)
* How to address: Use manual check of session handling in the code, e.g., exposes session IDs in the URL, does not rotate session IDs after successful login, does not properly invalidate session IDs.
* How to prevent: Session IDs should not be in the URL, be securely stored and invalidated after logout, idle, and absolute timeouts.
# Broken authentication
* How to address: Use manual means and exploit by using automated tools with password lists and dictionary attacks.
* How to prevent: Implement multi-factor authentication to prevent automated, credential stuffing, brute force, stolen credential reuse attacks, protecting credentials in transit, and all passwords must be stored in either hashed or encrypted form to protect them from exposure, regardless of where they are stored.
# Broken access control
* How to address: Use manual testing to detect missing or ineffective access control, including HTTP method (GET vs PUT, etc), controller, direct object references, etc.
* How to prevent: Users cannot act outside of their intended permissions, enforcement of model access control of ownership record, and web server directory listing, file metadata and backup files should be disable in order not expose the web roots.


# References
* OWASP Top 10 - 2017 The Ten Most Critical Web Application Security Risks (https://www.owasp.org/images/b/b0/OWASP_Top_10_2017_RC2_Final.pdf )
* XSS (Cross Site Scripting) Prevention Cheat Sheet (https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet )
* Carnegie Mellon University: Understanding Malicious Content Mitigation for Web Developers (https://resources.sei.cmu.edu/library/asset-view.cfm?assetid=496719 )

