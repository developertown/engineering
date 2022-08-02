# Security

## HTTP Headers

[https://securityheaders.com/](https://securityheaders.com/)

* Strict-Transport-Security
* Content-Security-Policy
* X-Frame-Options
* X-Xss-Protection
* X-Content-Type-Options
* Referrer-Policy


### Strict-Transport-Security

HTTP Strict Transport Security (HSTS) is a policy mechanism that allows a web server to enforce the use of TLS in a compliant User Agent (UA), such as a web browser. HSTS allows for a more effective implementation of TLS by ensuring all communication takes place over a secure transport layer on the client side. Most notably HSTS mitigates variants of man in the middle (MiTM) attacks where TLS can be stripped out of communications with a server, leaving a user vulnerable to further risk.

In order to implement HSTS a host must declare to a UA that it is a HSTS Host by issuing a HSTS Policy. This is done with the addition of the HTTP response header `Strict-Transport-Security: max-age=31536000`

### Content-Security-Policy

The CSP header allows you to define a whitelist of approved sources of content for your site. By restricting the assets that a browser can load for your site. CSP can act as an effective countermeasure to XSS attacks.

### X-Frame-Options

The X-Frame-Options header (RFC), or XFO header, protects your visitors against clickjacking attacks.

`X-Frame-Options: SAMEORIGIN`

### X-Xss-Protection

This header is used to configure the built in reflective XSS protection found in Internet Explorer, Chrome and Safari (Webkit).

`X-Xss-Protection: 1; mode=block`

### X-Content-Type-Options

Prevents Google Chrome and Internet Explorer from trying to mime-sniff the content-type of a response away from the one being declared by the server. It reduces exposure to drive-by downloads and the risks of user uploaded content that, with clever naming, could be treated as a different content-type, like an executable.

`X-Content-Type-Options: nosniff`

### Referrer-Policy

## TLS

[https://observatory.mozilla.org/](https://observatory.mozilla.org/)