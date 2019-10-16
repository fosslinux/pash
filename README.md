# pash

pash, ssh crossed with pass to make a ssh key system.

It uses the pass password manager to store passwords for the keys.

Features:
  - Only requires you to know one password; your 'pass' password.
  - A (not very secure) form of 2FA; you need your 'pass' password as well as the ssh key to ssh to the host.
  - One ssh key per host; so if one gets compromised, they do not get access to all hosts.

fosslinux (the developer) still uses this many times a day, reliabily.

A security issue you should be aware of is that the password *may* remain in memory after the script finishes, as the password is temporarily stored in a variable. There is no easy way around this; see https://stackoverflow.com/questions/38624253/how-to-overwrite-the-memory-segment-of-a-variable-in-bash and https://stackoverflow.com/questions/45000206/secure-erase-of-a-bash-environmental-variable.
