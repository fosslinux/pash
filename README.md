# pash

pash, ssh crossed with pass to make a ssh key system.

It uses the pass password manager to store passwords for the keys.

Features:
  - Only requires you to know one password; your 'pass' password.
  - A (not very secure) form of 2FA; you need your 'pass' password as well as the ssh key to ssh to the host.
  - One ssh key per host; so if one gets compromised, they do not get access to all hosts.

fosslinux (the developer) still uses this many times a day, reliabily.
