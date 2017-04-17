### Change SSH Port

- SSH Config
- ``/etc/ssh/sshd_config``
- Port
- Restart ``systemctl restart sshd`` ``service sshd restart``

### Open port(s), service(s) on firewall

- ``firewall-cmd --permanent --zone=public --add-port=xxxx-yyyy/tcp`` (``--add-service=ssh``, ``/udp``)
- ``firewall-cmd --reload``
