---
layout: page
title: Usage - Help
navigation: 2
---

# Foxy (Pentester APP)

## General Help

```
help command
```
```
● [Basic]:

    clear          : clear cmd
    history        : show Foxy command history
    ls             : list files in current directory
    pwd            : print current directory
    cd <dir>       : open folder
    ping <host>    : ping host

● [Advanced]:
    list                : list avaliable payloads
    set payload <pn>    : set payload to start
    back                : back to Foxy

```
list command
```
- list command will show you avaliable payloads table.
```

**Here is the sample of** `foxy::net::port-scanner` **payload usage :**

Set payload to start :
```
[Foxy] > set payload foxy::net::port-scanner
```

`show` Command to see setted variables. (It is null at start.)

```
___________________________________________
● Config :

    Target :

● Set Help :

    set target:<target_ip>
___________________________________________
```

Set target to start exploit.
```
[foxy::net::port-scanner] > set target:5.2.84.221
```

Output will show you setted information :

```
target ==> 5.2.84.221
```

And you are ready to run (exploit) :

```
[foxy::net::port-scanner] > run
```

Output will be like this.

```
[*] Starting port scanning for 5.2.84.221.

	Port	Action	Service
	21	open	ftp
	80	open	http
```

This is just port scanner. You can use other payloads easily. Same logic. Use help command...
