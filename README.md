# openemr_RCE_5.0.2
## Description
This exploit drop a web shell on an OpenEMR v5.0.2.1 CMS. At the end, GET the URL and run a netcat listener on the LHOST:LPORT. You will be able to do a Remote
Code Execution on this server.
You need to wait the Admin to change his password and it'll trigger the XSS.

## Usage
```
usage: openemr_exploit.py [-h] [-d [DIRECTORY]] -rh RHOST [-rp [RPORT]] [-vh [VHOST]] -lh LHOST -lp LPORT [-wp [WPORT]]

optional arguments:
  -h, --help            show this help message and exit
  -d [DIRECTORY], --directory [DIRECTORY]
                        Root directory OpenEMR CMS
  -rh RHOST, --rhost RHOST
                        Remote server IP
  -rp [RPORT], --rport [RPORT]
                        Remote server PORT
  -vh [VHOST], --vhost [VHOST]
                        Remote server DOMAIN_NAME
  -lh LHOST, --lhost LHOST
                        Reverse shell IP
  -lp LPORT, --lport LPORT
                        Reverse shell PORT
  -wp [WPORT], --wport [WPORT]
                        Web Server PORT
```                        

## Authors
+ [Hato0](https://github.com/Hato0)
+ [BvThTrd](https://github.com/BvThTrd)

## References

+ [Blog](https://blog.sonarsource.com/openemr-5-0-2-1-command-injection-vulnerability?utm_medium=cpc&utm_source=twitter&utm_campaign=openemr&utm_term=security&utm_content=tofu)
+ [Youtube](https://www.youtube.com/watch?v=H8VWNwWgYJo&feature=emb_logo)
