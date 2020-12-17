# Certificate
Setup :material-menu-right: Information :material-menu-right: Certificate

**Certificate** management for public-key cryptography, such as:

* Customer Portal
* WebPhone
* TLS SIP
* WebRTC

ConnexCS provides certificates free of charge courtesy of **[Let's Encrypt](https://letsencrypt.org/)** or User Provided.

## Add Certificate
To add a certificate:

1. Click on the :fontawesome-plus: symbol.
2. See configuration details below. 

### Let's Encrypt

1. Enter the **Domain** name for this certificate. To allow ConnexCS to manage your certificates, you must ensure that the DNS records are set correctly so they are pointing to the correct server of ours.
2. Set **User Provided** to "No". 
3. Click **`Save`** and our system will provision the certificate for you.

Let's Encrypt renewals are managed automatically.

### User Provided

1. Enter the domain name for this certificate.
2. Ensure that you have user provided to set to "Yes".
3. Certificate and keys should be in PEM (base64 format).
4. Paste your **Certificate** starting with `-----BEGIN CERTIFICATE-----` and ending with `-----END CERTIFICATE-----`.
5. Paste your private **Key** starting with `-----BEGIN PRIVATE KEY-----` and ending with `-----END PRIVATE KEY-----`.
6. Paste in your **CA(Certificate Authority) Certificate** starting with `-----BEGIN CERTIFICATE-----` and ending with `-----END CERTIFICATE-----`.

Renewals for User Provided certificates are your responsibility.

## Checking Certificates

The Status column contains a :fontawesome-check: representing all checks having passed.

A problem is represented by :fontawesome-exclamation-triangle:. If you hover your mouse you will see a checklist explaining the issue.