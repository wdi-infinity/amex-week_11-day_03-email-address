# Unique Email Addresses

Practicing more about solving algorithms!

## The Problem:

Every email consists of a local name and a domain name, separated by the @ sign.

For example, in `ghadeer.alkathlan@generalassemb.ly`, `ghadeer.alkathlan` is the local name, and `generalassemb.ly` is the domain name.

Besides lowercase letters, these emails may contain '.'s or '+'s.

If you add periods ('.') between some characters in the local name part of an email address, mail sent there will be forwarded to the same address without dots in the local name. For example, `ghadeer.alkathlan@generalassemb.ly` and `ghadeeralkathlan@generalassemb.ly` forward to the same email address. (Note that this rule does not apply for domain names.)

If you add a plus ('+') in the local name, everything after the first plus sign will be ignored. This allows certain emails to be filtered, for example m.y+name@email.com will be forwarded to my@email.com. (Again, this rule does not apply for domain names.)

It is possible to use both of these rules at the same time.

Given a list of emails, we send one email to each address in the list. How many different addresses actually receive mails?

![email](https://seooasis.co.uk/wp-content/uploads/2015/03/Email-marketing-meme.jpg)

Example 1:
```
Input: ["mic.email+finn@generalassemb.ly","mic.e.mail+fi.nn@generalassemb.ly","usman+bashir@general.assemb.ly"]
Output: 2
Explanation: "micemail@generalassemb.ly" and "usman@general.assemb.ly" actually receive mails
```

Note:
1 <= emails[i].length <= 100
1 <= emails.length <= 100
Each emails[i] contains exactly one '@' character.
