# Log Book 4

## Task 1

## Task 2

## Task 3

## Task 4

## Task 5

## Task 6

---

## CTF 4

- **Wordpress version**: 5.8.1
- **Installed plugins + version**: Woocommerce 5.7.1
- **Possible users**: admin, Orval Sandford

This vulnerability is identified by the CVE-2021-34646.
It has a CVSS score of 7.5 and it's type is *Bypass a resctriction or similar*. ([CWE-330](https://cwe.mitre.org/data/definitions/330.html))
More information about this vulnerability can be found [here](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-34646) and [here](https://www.cvedetails.com/cve/CVE-2021-34646/?q=CVE-2021-34646).

After finding the CVE, we could search it in a exploit database. In this case we used [this](https://www.exploit-db.com/exploits/50299) database, where we found a exploit code that would help us break into the admin account without needing any kind of log in verification.

The program just needed the target website and a user id to run, and since we want to attack the admin account, we figured the user id must be either 0 or 1.
After running the given Python program, we obtained the following output:
(image here)

Then, all we needed to do was access the target website with the url generated by the program and we are inside the admin account.

After browsing through the website in admin mode, we found a private post that had the flag of the CTF.