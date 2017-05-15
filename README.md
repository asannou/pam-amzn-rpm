# Amazon RPM for PAM (Pluggable Authentication Modules)

## Build RPM Package

```
$ mv $PWD ~/rpmbuild
$ sudo yum-builddep SPECS/pam.spec
$ spectool -g -R SPECS/pam.spec
$ rpmbuild -bb --clean SPECS/pam.spec
```
