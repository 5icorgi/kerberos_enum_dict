# kerberos_enum_dict

枚举kerberos域用户的字典

以及更多用途...

# Usage

```
msf > use auxiliary/gather/kerberos_enumusers
msf auxiliary(kerberos_enumusers) > show actions
msf auxiliary(kerberos_enumusers) > set ACTION <action-name>
msf auxiliary(kerberos_enumusers) > show options
msf auxiliary(kerberos_enumusers) > run
```

# TOOLS

- [Krbguess](http://www.cqure.net/wp/tools/password-recovery/krbguess/)

```
Java –jar kerbguess.jar –r [domain] –d [user list] –s [DC IP]
```

- Nmap [krb5-enum-users](https://nmap.org/nsedoc/scripts/krb5-enum-users.html) NSE Script

```
Nmap –p 88 –script-args krb5-enum-users.realm=’[domain]’,userdb=[user list] [DC IP]
```

- [KerberosUserEnum](https://github.com/360-A-Team/KerberosUserEnum)

```
./Enum.py --file=/tmp/usernames --dcip=192.168.88.1 --domain=TESTDOMAIN --port=88
```
