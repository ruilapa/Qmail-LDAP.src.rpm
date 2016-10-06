INSTALL

1 - get an qemu, vmware, ..., clean RH based system (honestly)
2 - rpm -i {attached_rpms}
3 - edit SOURCES/qmail-ldap.config
4 - download to your SOURCES ( they exist, but empty  ):
- daemontools-0.76.tar.gz
- qmail-1.03.tar.gz
- ucspi-tcp-0.88.tar.gz
from DJB site
5 - start building, without being root.
    rpmbuild -bb {each_spec}


NOTES

- qmail default install path is /var/qmail
- UID's and GID's are static
- supervised daemons are on /var/lib/supervise.d
- supervise-ldap-0.1.tgz as the init's


TODO

- integrate patches since  20050401a
- change default install path
- dinamic UID/GID - there is a patch from Bruce Guenter (?)
- ways to do some of the "black magic" stuff in a better way
- insert tarpit control
- insert
- cleaning code

