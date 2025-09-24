
# QUIC and ECH

This directory has the .tex and .bib sources.

To update ietf.bib (for me, ymmv) for some RFC or I-D, I
installed rfcbibtex, but since I'll forget how to use it:

```bash
$ pipenv run rfcbibtex rfc8446 draft-ietf-tls-esni -o new.bib
$ cat new.bib >>ietf.bib
```

