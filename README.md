# Ansible-Installation-Guide
Install Ansible in your RHEL system within 10 minutes.

<pre>
────────────────────────────────────────────────────────
────────────────────────────────────────────────────────

╔═╗┌┐┌┌─┐┬┌┐ ┬  ┌─┐  ╔═╗┌─┐┌┬┐┬ ┬┌─┐  ╦ ╦┌─┐┬  ┌─┐┌─┐┬─┐
╠═╣│││└─┐│├┴┐│  ├┤   ╚═╗├┤  │ │ │├─┘  ╠═╣├┤ │  ├─┘├┤ ├┬┘
╩ ╩┘└┘└─┘┴└─┘┴─┘└─┘  ╚═╝└─┘ ┴ └─┘┴    ╩ ╩└─┘┴─┘┴  └─┘┴└─

────────────────────────────────────────────────────────
────────────────────────────────────────────────────────

+ Note : ------------------------------+
|                                      |
| * In rhel, 'yum' must be configured. |
|                                      |
+--------------------------------------+
</pre>
```
[0] ┬ Install epel repository:
    ├─[*] $ yum install -y https://download-ib01.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm
    └─[*] $ yum makecache
```

```
[1] ┬ Download some important packages:
    ├─[*] Use this link & download in your system: https://shorturl.at/evX14
    │ [OR] 
    └─[*] 1. Go to https://access.redhat.com/downloads/content/package-browser
          2. Search for keyword 'ansible'.
          3. Download the package - ansible-2.9.27-1.el8ae.noarch.rpm
          4. Search for keyword 'sshpass'.
          5. Download the package - sshpass-1.06-3.el8ae.x86_64.rpm
          6. Put both package in your root directory.
```

```
[2] ┬ Install python version 3 and some dependencies:
    ├─[*] $ yum install python36 -y
    └─[*] $ yum install python3-libmodulemd -y
```

```
[3] ┬ Install sshpass & ansible:
    ├─[*] $ yum install sshpass-1.06-3.el8ae.x86_64.rpm -y
    └─[*] $ yum install ansible-2.9.27-1.el8ae.noarch.rpm -y
```

```
$ ansible --version
```

```
All Done !?!
```
