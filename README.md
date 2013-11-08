PuTTY-CAC
=========

Secure shell client with support for US Government Smartcards and other X.509 certificates.

This is a fork of PuTTY.  It breaks much of the delictious goodness of
the original PuTTY, in that it only builds for Windows, and is only
known to build correctly with Microsoft Visual C, at this time.

But it supports the DoD Common Access Card (CAC) and a number of other smartcards.  

PuTTY-CAC is now updated to 0.63.  It fixes four security holes in 0.62
and before: vuln-modmul, vuln-signature-stringlen,
vuln-bignum-division-by-zero, private-key-not-wiped.  This version also
includes a more simplified interface for pageant when adding CAPI Certs.
The PKCS11 API has been removed from all applications in this PuTTY-CAC
Suite due to complications I was having with the code.  However, CAPI
support is fully functional which is the main premise behind PuTTY-CAC
anyways.  I have included compiled version of the PuTTY-CAC Suite that
can be found in the EXECUTABLES folder.  This includes all parts of the
PuTTY Suite except for PuTTYTEL.  If you choose to compile it yourself
you will need to use the MakeFile.vc as I did not update or support the
another MakeFile.* files.