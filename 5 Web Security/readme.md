# LAB 5

Networks and Systems Security
Week 05
Web Security

## Aims of the Seminar

In this workshop, we'll dive into the essential
principles Web application vulnerability scanning. Web application vulnerability
scanning is the process of using automated tools to identify security weaknesses in
web applications. These scanners work by sending a variety of requests to a web
application and analysing the responses to find potential vulnerabilities. This is a
crucial part of a web security audit, as it helps to identify and fix security holes before
they can be exploited by attackers.

## Resources

- Wapiti Docs: https://wapiti-scanner.github.io/
- OWASP Juice Shop: https://owasp.org/www-project-juice-shop/
- Google Gruyere: https://google-gruyere.appspot.com/
- Full Wapiti GitHub: https://github.com/wapiti-scanner/wapiti

## 🛑⚠️Ethical Reminder⚠️

### Never scan a website without explicit permission.

The apps below are designed for security testing—they are legal, safe, and
maintained for education.

Do not scan any other site during this workshop.

## Final Conclusion and Reflection

This workshop had me explore automated web vulnerability scanning with Wapiti, deepening my understanding of assessing a sites security. Scanning my own Google Gruyere instance showed how quickly a tool can identify common issues such as missing security headers, insecure cookies, reflected XSS, and stored XSS. These findings reinforced the importance of website security due to how easily vulnerabilities can be exposed.

I found going onto my Gruyere instance to try finding and exploiting the vulnerabilities found by the scanner to be very enjoyable. This also showing the limits of scanners, with it not detecting the privilege-escalation flaw that allowed me to grant myself admin rights simply by altering a URL parameter. This inforces the fact that real security assessment still requires human expertise and analysis. Besides this, my knowlage on main secutity concepts like XSS are now much more grounded, having exploited these vulnerabilites myself.

Overall, this workshop strengthened my understanding of both the value and the limitations of automated scanning. It made me more aware of the importance of defence-in-depth and secure coding practices, but also more confident in my ability to test and reason about web application behaviour myself.
