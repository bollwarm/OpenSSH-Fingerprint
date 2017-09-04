# OpenSSH-Fingerprint

penSSH-Fingerprint - A module for openssh key Fingerprint create support md5 and sha256.

## INSTALLATION

To install this module, run the following commands:

	perl Makefile.PL
	make
	make test
	make install

## Example

     use OpenSSH::Fingerprint;
     use use MIME::Base64;
     my $file=shift;
     my $resutlt= unbase64($file);

     print "md5 fingerpint: ",md5_sum($_ ),"\n"  for(@{$resutlt});
     print "sha265 fingleprint: ",encode_base64(sha256($_ ))  for(@{$resutlt});

## The result

    perl sshfingerprint.pl aaa.pub

    md5 fingerpint: 4b:12:23:8a:95:rt:ec:da:43:fc:aa:0b:1a:e6:6a:2f
    sha265 fingleprint: sfeQQGLlTi5j69KMzEkLmK9f78/CGtVk2a8N8pDfV88=


## SUPPORT AND DOCUMENTATION

After installing, you can find documentation for this module with the
perldoc command.

    perldoc OpenSSH::Fingerprint

You can also look for information at:

###  RT, CPAN's request tracker (report bugs here)
        http://rt.cpan.org/NoAuth/Bugs.html?Dist=OpenSSH-Fingerprint

### AnnoCPAN, Annotated CPAN documentation
        http://annocpan.org/dist/OpenSSH-Fingerprint

### CPAN Ratings
        http://cpanratings.perl.org/d/OpenSSH-Fingerprint

### Search CPAN
    
    http://search.cpan.org/dist/OpenSSH-Fingerprint/

### Git repo

[github] (https://github.com/bollwarm/OpenSSH-Fingerprint.git)

[oschina] (https://git.oschina.net/ijz/OpenSSH-Fingerprint.git)


## LICENSE AND COPYRIGHT

Copyright (C) 2017 ORANGE

This program is released under the following license: Perl

