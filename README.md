# TLS-knowledge

What is CAA?

A Certification Authority Authorization (CAA) record is used to specify which certificate authorities (CAs) are allowed to issue certificates for a domain.

The CAA record consists of a flags byte and a tag-value pair referred to as a ‘property’.

The canonical representation is:

```
CAA <flags> <tag> <value>
```
The RFC currently defines 3 available tags:

* issue: explicity authorizes a single certificate authority to issue a certificate (any type) for the hostname.

* issuewild: explicity authorizes a single certificate authority to issue a wildcard certificate (and only wildcard) for the hostname.

* iodef: specifies a URL to which a certificate authority may report policy violations.
