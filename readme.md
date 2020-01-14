```
wget https://raw.githubusercontent.com/melvin-suter/selinux-postfix-milter-fix/master/postfix_milter_fix.te
checkmodule -M -m -o postfix_milter_fix.mod postfix_milter_fix.te
semodule_package -o postfix_milter_fix.pp -m postfix_milter_fix.mod
semodule -i postfix_milter_fix.pp
```
