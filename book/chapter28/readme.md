Table of Contents

28.1 Reference Security Sections in Other Chapters . . . . . . . . . . . . . . 333
28.2 Harden Your Servers . . . . . . . . . . . . . . . . . . . . . . . . . . . . 333
28.3 Know Django’s Security Features . . . . . . . . . . . . . . . . . . . . . 334
28.4 Turn Off DEBUG Mode in Production . . . . . . . . . . . . . . . . . 334
28.5 Keep Your Secret Keys Secret . . . . . . . . . . . . . . . . . . . . . . . 334
28.6 HTTPS Everywhere . . . . . . . . . . . . . . . . . . . . . . . . . . . 335
28.6.1 Use Secure Cookies . . . . . . . . . . . . . . . . . . . . . . . . 337
28.6.2 Use HTTP Strict Transport Security (HSTS) . . . . . . . . . . 337
28.6.3 HTTPS Configuration Tools . . . . . . . . . . . . . . . . . . . 338
28.7 Use Allowed Hosts Validation . . . . . . . . . . . . . . . . . . . . . . . 339
28.8 Always Use CSRF Protection With HTTP Forms That Modify Data . . 339
28.9 Prevent Against Cross-Site Scripting (XSS) Attacks . . . . . . . . . . . 339
28.9.1 Use format_html Over mark_safe . . . . . . . . . . . . . . . . 339
28.9.2 Don’t Allow Users to Set Individual HTML Tag Attributes . . . 340
28.9.3 Use JSON Encoding for Data Consumed by JavaScript . . . . . 340
28.9.4 Beware Unusual JavaScript . . . . . . . . . . . . . . . . . . . . 340
28.9.5 Add Content Security Policy Headers . . . . . . . . . . . . . . 340
28.9.6 Additional Reading . . . . . . . . . . . . . . . . . . . . . . . . 341
28.10 Defend Against Python Code Injection Attacks . . . . . . . . . . . . . 341
28.10.1 Python Built-Ins That Execute Code . . . . . . . . . . . . . . . 341
28.10.2 Python Standard Library Modules That Can Execute Code . . . 341
28.10.3 Third-Party Libraries That Can Execute Code . . . . . . . . . . 342
28.10.4 Be Careful With Cookie-Based Sessions . . . . . . . . . . . . . 342
28.11 Validate All Incoming Data With Django Forms . . . . . . . . . . . . . 343
28.12 Disable the Autocomplete on Payment Fields . . . . . . . . . . . . . . 344
28.13 Handle User-Uploaded Files Carefully . . . . . . . . . . . . . . . . . . 344
28.13.1 When a CDN Is Not an Option . . . . . . . . . . . . . . . . . 344
28.13.2 Django and User-Uploaded Files . . . . . . . . . . . . . . . . . 345
28.14 Don’t Use ModelForms.Meta.exclude . . . . . . . . . . . . . . . . . . . 346
28.14.1 Mass Assignment Vulnerabilities . . . . . . . . . . . . . . . . . 348
28.15 Don’t Use ModelForms.Meta.fields = ”__all__” . . . . . . . . . . 348
28.16 Beware of SQL Injection Attacks . . . . . . . . . . . . . . . . . . . . . 348
28.17 Don’t Store Unnecessary Data . . . . . . . . . . . . . . . . . . . . . . . 349
28.17.1 Never Store Credit Card Data . . . . . . . . . . . . . . . . . . 349
28.17.2 Don’t Store PII or PHI Unless Required (By Law) . . . . . . . 349
28.18 Monitor Your Sites . . . . . . . . . . . . . . . . . . . . . . . . . . . . 350
28.19 Keep Your Dependencies Up-to-Date . . . . . . . . . . . . . . . . . . 350
28.20 Prevent Clickjacking . . . . . . . . . . . . . . . . . . . . . . . . . . . . 350
28.21 Guard Against XML Bombing With defusedxml . . . . . . . . . . . . 351
28.22 Explore Two-Factor Authentication . . . . . . . . . . . . . . . . . . . 351
28.23 Embrace SecurityMiddleware . . . . . . . . . . . . . . . . . . . . . . . 352
28.24 Force the Use of Strong Passwords . . . . . . . . . . . . . . . . . . . . 352
28.25 Don’t Prevent Copy/Pasting of Password . . . . . . . . . . . . . . . . . 353
28.26 Give Your Site a Security Checkup . . . . . . . . . . . . . . . . . . . . 353
28.27 Put Up a Vulnerability Reporting Page . . . . . . . . . . . . . . . . . . 353
28.28 Never Display Sequential Primary Keys . . . . . . . . . . . . . . . . . . 353
28.28.1 Lookup by Slug . . . . . . . . . . . . . . . . . . . . . . . . . . 354
28.28.2 UUIDs . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 354
28.29 Upgrade Password Hasher to Argon2 . . . . . . . . . . . . . . . . . . . 356
28.30 Use SRI When Loading Static Assets From External Sources . . . . . . 356
28.31 Reference Our Security Settings Appendix . . . . . . . . . . . . . . . . 358
28.32 Review the List of Security Packages . . . . . . . . . . . . . . . . . . . 358
28.33 Keep Up-to-Date on General Security Practices . . . . . . . . . . . . . 358
28.34 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 359
