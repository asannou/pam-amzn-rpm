# Amazon RPM for PAM (Pluggable Authentication Modules)

## Build RPM Package

```
$ sudo yum-builddep SPECS/pam.spec
$ spectool -C SOURCES -g SPECS/pam.spec
$ rpmbuild --define "_topdir $PWD" -bb --clean SPECS/pam.spec
```

## Update SRPM

```
$ get_reference_source -p pam
$ rpm --define "_topdir $PWD" -ivh /usr/src/srpm/debug/pam-X.X.X-X.X.amzn1.src.rpm
```
