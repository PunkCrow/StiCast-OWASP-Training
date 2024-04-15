# StiCast-OWASP-Training

This project involves a comprehensive study and mitigation of vulnerabilities associated with the OWASP Top 10 web application security risks. Utilizing "StiCast!", a web application developed initially for the study of collective intelligence in forecasting, this research demonstrates the practical implications of various security vulnerabilities and their mitigations. "StiCast!" was intentionally designed with vulnerabilities to serve as a testbed for demonstrating attack techniques and their respective mitigation strategies.

## Project Setup

### Requirements
- Docker
- Git

### Deployment

To deploy the project, clone the repository and use Docker to launch both the vulnerable and secured versions of "StiCast!":

```bash

git clone http://gitlab.comics.unina.it/AT-Projects/StiCast.git
cd StiCast/NS_StiCast
docker-compose up
```

### Access the application:

- Vulnerable version: http://localhost:8080/sticast_ko
- Secured version: https://localhost:8443/sticast_ok

You can create a new account or using the following credentials to access the vulnerable version:
- Username: pippo
- Password: pippo123

## Vulnerabilities and Mitigations

This study covers various vulnerabilities as categorized by the OWASP Top 10 list. Each section details a type of vulnerability, demonstrates it with practical scenarios using the intentionally vulnerable "StiCast!" webapp, and discusses effective mitigation techniques implemented in the secure version.

### XSS (Cross-Site Scripting)
Includes Stored, Reflected, and DOM-based XSS attacks with detailed examples, attack scenarios, and mitigation steps.

### CSRF (Cross-Site Request Forgery)
Demonstrates CSRF attacks through practical scenarios and discusses mitigation strategies such as using tokens and setting SameSite cookie attributes.

### SQL Injection
Explores various forms of SQL Injection attacks and their prevention, emphasizing the importance of using parameterized queries.

### Sensitive Data Exposure / Crypographic Failures
Discusses encrypting sensitive data transmissions using HTTPS and secure password storage mechanisms.

### Broken Authentication
This project also delves into the prevalent issue of Broken Authentication. Broken Authentication occurs when attackers are able to compromise user accounts, keys, or session tokens to assume user identities. The examples provided in this study demonstrate how attackers exploit common issues such as predictable login credentials, poorly protected session tokens, and flaws in logout mechanisms.

This project also delves into the prevalent issue of Broken Authentication. Broken Authentication occurs when attackers are able to compromise user accounts, keys, or session tokens to assume user identities. Implemented 2FA, brute force account blocking, and token recovery password.

## Detailed Vulnerability Descriptions and Exploitation Scenarios

For an in-depth understanding of the security vulnerabilities covered in this project, along with real-case exploitation scenarios, you can check the accompanying PDF document. It provides a comprehensive analysis of each vulnerability, outlines methods of exploit, and offers a rich set of resources for further learning and mitigation strategy.

The PDF includes step-by-step examples of how each vulnerability can be exploited, reflecting real-world attack patterns that can help both developers and security professionals understand the intricacies of web security.

To delve into the details, please refer to the [StiCastOWASPTraining.pdf](StiCastOWASPTraining.pdf) included in this repository.

## Contributing

Contributions to the study are welcome. If you have updates, additional vulnerabilities to discuss, or improvements to mitigation strategies, please fork the repository and submit a pull request.
