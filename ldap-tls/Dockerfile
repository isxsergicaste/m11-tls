# Version: 0.0.1
# @Sergi Castella
# ldapserver
# -------------------------------------
FROM fedora:27
LABEL author="@edt ASIX M06 Curs 2018-2019"
LABEL description="ldapserver"
RUN dnf -y install procps openldap-clients openldap-servers
RUN mkdir /opt/docker
COPY * /opt/docker/
RUN chmod +x /opt/docker/install.sh /opt/docker/startup.sh
WORKDIR /opt/docker
CMD ["/opt/docker/startup.sh"]
