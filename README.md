# mirrorScript
Script to change kali repository mirror

http://http.kali.org redirects you to the closest available mirror based on your physical location.
Most of the time the servers may experience heavy load, thus slowing down upgrades even with fast connection.
This script lets you rank(based on the server's ping) and choose an alternative mirror and override it.

You can find the original mirror list here [Kali Mirrors](https://http.kali.org/README.mirrorlist)

# Requirements
Kali Linux,
Python2.7 (comes pre-bundled)

# Usage
>Run the script in privilege mode, such that sources.list could be edited

> **$ sudo python mirrorscript.py**

#---------------------------------------------------------------------------#
UPDATED: 06/MAY/2018 To Execute on Python3+
(Python 3.6.4)

PROBLEM Running on Python3:
returns error:
 
when File "mirrorscript.py", line 11
    print ""
           ^
SyntaxError: Missing parentheses in call to 'print'. Did you mean print("")?

#------------------------------------------------------------
Solution: 
Python3+ versions now use print("") instead of print ""
-all print methods used in mirrorscript.py are now converted to new required format
#------------------------------------------------------------