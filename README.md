# Applcation-Analysis




APPLICATION ANALYSIS

7. Perform an application analysis:
i) Ask yourself 6 Big Questions:
a) How does the app pass data? parameters(?next=/test/tester) or endpoints(/next/test/tester).
b) How does the app refer to users?- uuid, email, username, uid — and where? cookies, API calls.
c) Does the site have multi-tenancy or user levels? admin(cms/framework), tenant/account-admin, tenant/account-user, tenant/account-viewer, unauthenticated functionality.
d) Does the site have a unique threat model? eg PII sensitive to only this webapp.
e) Has there been past security research and vulnerabilities to give an insight on what vulnerabilities to look for.
f) How does the app mitigate against XSS, CSRF, Code Injection, SQL, Template.

8. Do some spidering to find out more about the app, to get more endpoints, to get more directories.

9. Target the ‘hot areas’ — Heat Mapping:
i) Upload functions — Integrations from 3rd party: XSS , Self Uploads: { { XML based( DOCX/PDF ): { SSRF, XXE, XSS } }, Images: { XSS, Shell: { Name, Binary header, Metadata } }, where is data stored: S3 params.
ii) Content-Types — Look for multipart forms: { Shell, Injections, ++ }, Look for Content-Type XML: { XXE }, Look for Content-Type json: { API vulnerabilities — mass assignment, information disclosure, Improper Asset Management, Broken Access Control }
iii) APIs — Hidden Methods, Lack of auth.
iv) Account Section — Profile: { Stored XSS }, Application Custom Fields: { Stored XSS, SSTI}.
v) Errors — exotic injections, App DoS.
vi) Paths or URLs passed as values — SSRF and redirects.

10. Now start a deeper assessment. Use a checklist to make sure you test for everything as you check them off. You can employ the help of the OWASP testing guide and spreadsheets to test for as many applicable groups of vulnerabilities as you can.

