1. Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did the firm want you to resolve?

Artemis Financial is a finance company that requires higher security for its software application. Protecting sensitive data transmissions and data integrity through cryptographic hashing was the prime concern of the company that it wished to address. The project involved enhancing software security through the addition of an encryption algorithm, generating security certificates, incorporating a secure checksum function, and verifying communications security.

2. What did you do well when you found your client's software security vulnerabilities? Why does one need to code securely? What is the value that software security adds to the overall health of a company?

I was successful in finding and resolving security vulnerabilities in the software of Artemis Financial by:

•	Implementing SHA-256 hashing for secure data integrity verification.
•	Enforcing HTTPS communication to prevent unauthorized data interception.
•	Performing dependency security scans to remove risks from outdated third-party libraries.

Secure coding is necessary to prevent data breaches, protect sensitive financial information, and meet industry security standards. Strong security increases client trust protects the company reputation and minimizes potential legal or financial ramifications.

3. What part of the vulnerability analysis was challenging or valuable to you?

The toughest part of the test was remedying vulnerabilities in third-party dependencies found using OWASP Dependency-Check. There were several critical and high-severity vulnerabilities found in Spring Boot, Hibernate Validator, and Jackson Databind. Since dependency management must be carried out carefully so as not to disrupt functionality, I had to research and ensure that upgrading to higher versions would not lead to compatibility issues.4. Explain how you implemented layers of security. Going forward, what would you use to identify vulnerabilities and decide on which mitigation strategies to use?

I implemented security in multiple layers of defense:

•	Data encryption uses SHA-256 to prevent tampering.
•	Securing HTTPS connections to encrypt all data in transit.
•	Input validation and exception handling to prevent injection attacks.
•	Scanning dependencies for vulnerabilities so that the application doesn't rely on insecure libraries.

In the future, I would continue to use OWASP Dependency-Check, SonarQube for static code analysis, and Burp Suite for penetration testing to analyze vulnerabilities and select appropriate mitigation strategies.

5. How did you verify the software application and code were functional and secure? How did you verify whether you introduced new vulnerabilities when you refactored the code?

I verified functionality and security through a few checking steps:

•	Functional Testing: Verified that the /checksum endpoint was processing and returning SHA-256 hashes appropriately.
•	Secure Communications Testing: Confirmed that HTTPS was forced, and data encryption was on.
•	Dependency Scanning: Utilized OWASP Dependency-Check to scan for new security vulnerabilities introduced by changes.

With frequent testing and log analysis, I could confirm no new vulnerabilities were introduced.
6. What resources, tools, or coding practices did you use that may be useful for future assignments or tasks?

Some of the major tools and resources used in this project include:

•	OWASP Dependency Check – Identified third-party library vulnerabilities using this.
•	Spring Boot Security Best Practices – Implemented secure cryptographic functions based on this.
•	Java Keytool – Generated self-signed security certificates for authentication.
•	HTTPS Configuration – Enforced encrypted data communication on a secured protocol.

These practices are those of secure coding and will serve you well for future software development work.

7. Employers sometimes ask for examples of work that you have done to prove your skill, knowledge, and experience. What might you show future employers from this assignment?

•	Use of secure cryptographic hashing with SHA-256.
•	Refactoring the code to introduce HTTPS security for encrypted data transfer.
•	Performing security tests with OWASP Dependency-Check to prevent vulnerabilities.
•	Applying industry-standard secure coding conventions to prevent cyber-attacks.
