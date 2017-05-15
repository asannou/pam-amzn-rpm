# Amazon RPM for PAM (Pluggable Authentication Modules)

## Build RPM Package

```
$ mv $PWD $HOME/rpmbuild
$ sudo yum-builddep SPECS/pam.spec
$ spectool -g -R SPECS/pam.spec
$ rpmbuild -bb --clean SPECS/pam.spec
```

## Update SRPM

```
$ get_reference_source -p pam
$ rpm -ivh /usr/src/srpm/debug/pam-X.X.X-X.X.amzn1.src.rpm
```
