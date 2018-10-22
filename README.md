**Admin Panel Finder**

Admin Panel Finder scans the target web site's administration panel by brute force. Save sites that provide http 200 response code. Privileged http 200 calls the input form in the links and warns the user when found. Modifies the User Agent in each connected request. Wordlist size and scan speed can be adjusted. Scan speed is increased by threading.

*This program was made for pentests. The user is responsible for all illegal use. The program author is not responsible for illegal use.*

**Usage:**
 - Download and install Python modules `pip3 install -r requirements.txt`
 - See all parameters or help: `sudo python3 panelfinder.py -h`

 - Standart Scan: sudo python3 panelfinder.py -u [target_web_site]

e.g. `sudo python3 panelfinder.py -u https://www.example.com`
 
 - Change Wordlist Size: sudo python3 panelfinder.py -u [target_web_site] -w [word_list_size]

e.g. `sudo python3 panelfinder.py -u https://www.example.com -w wordlist-big.txt`
 
 - Change Scan Speed: sudo python3 panelfinder.py -u [target_web_site] -w [word_list_size] -s [slow_or_normal_or_aggressive]
 
 Slow: 2 requests in 1 second, sleep2  seconds
 Normal: 5 requests in 1 seconds, sleep 2 seconds
 Aggressive: No limit

e.g. `sudo python3 panelfinder.py -u https://www.example.com -s aggressive`
