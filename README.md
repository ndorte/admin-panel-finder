**Admin Panel Finder**

Admin panel finder is a tool that tries to find the management panel of the target website by the brute-force method.
For URLs tested, the HTTP status code 200 saves, and at the same time, it looks for "login form" in the source code on the pages.

*This program was made for pentests. The user is responsible for all illegal use. The program author is not responsible for illegal use.*

**Usage:**
 - Download and install Python modules `pip3 install -r requirements.txt`
 - See all parameters or help: `sudo python3 panelfinder.py -h`

 - Standart Scan: sudo python3 panelfinder.py -u [target_web_site]

e.g. `sudo python3 panelfinder.py -u https://www.example.com`
 
 - Change Wordlist Size: sudo python3 panelfinder.py -u [target_web_site] -w [word_list_size]

e.g. `sudo python3 panelfinder.py -u https://www.example.com -w wordlist-big.txt`
 
 - Change Scan Speed: sudo python3 panelfinder.py -u [target_web_site] -w [word_list_size] -s [slow_or_normal_or_aggressive]
 
 **Slow:** 1 requests in 1 second, sleep 2 seconds | 
 **Normal:** 5 requests in 1 second, sleep 1 seconds | 
 **Aggressive:** No limit

e.g. `sudo python3 panelfinder.py -u https://www.example.com -s aggressive`
