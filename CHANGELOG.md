Changes
=======
v4.1.0 (07.07.2023)
---------------------------
-   Added `--sniff skipsizes=25:60:101:...`: allow skipping redirect to 200 OK pages which not found
-   Fix `--sniff skipempty`: increase condition value to detect empty content <= 500 bytes detect as empty page instead of 100 bytes
-   Fix `ResponseError: Unknown response status : 525`: added to define incorrect SSL handshakes
-   Fix `Object of type HTTPHeaderDictItemView is not JSON serializable`: if `--debug` set `3`
-   Fix `--accept-cookies` param. (Accept and route cookies from responses)
-   Fix response encode failed`('Received response with content-encoding: gzip, but failed to decode it.', error('Error -3 while decompressing data: incorrect header check'))`
-   Added `+20` new directories to internal wordlist
-   Added `+74242` new subdomains to internal wordlist
-   Optimize internal wordlist directories.txt list (sort, removed trash lines)

v4.0.61 (30.06.2023)
---------------------------
-   Added +1007 directories
-   Optimize directories.txt list (sort, removed trash lines)
-   Fix [#ISSUE-64](https://github.com/stanislav-web/OpenDoor/issues/64) HTTPConnection.__init__() got an unexpected keyword argument 'cert_reqs'

v4.0.6 (26.06.2023)
---------------------------
-   Re-create documentation portal. Keep docs up to date. Publish on Pypi

v4.0.5 (25.06.2023)
---------------------------
-   Fix unit tests and resolve dev requirements

v4.0.4-stable (24.06.2023)
---------------------------
-   Fix unit tests and resolve dev requirements

v4.0.3 (24.06.2023)
-------------------
-   Fix [#ISSUE-44](https://github.com/stanislav-web/OpenDoor/issues/44) ignore invalid SSL by default

v4.0.2 (23.06.2023)
-------------------
-   Python 3.11 launch fix [#ISSUE-58](https://github.com/stanislav-web/OpenDoor/issues/58) added encoding to setup.py 

v4.0.1-beta (23.02.2021)
------------------------
-   Python 2.6,2.7 is unsupported
-   Update directories.dat  36994 -> 37019
-   [enhancement] [#PR-40](https://github.com/stanislav-web/OpenDoor/issues/40) added encoding to setup.py 
-   [bugfix] [#PR-48](https://github.com/stanislav-web/OpenDoor/issues/48) Python 3.9 / 3.10 compatibility
-   [bugfix] [#PR-20](https://github.com/stanislav-web/OpenDoor/issues/20) No timeout setup in request
-   [enhancement] [#PR-36](https://github.com/stanislav-web/OpenDoor/issues/36) Feature Request: Show only found items

v3.4.481-stable (02.10.2017)
----------------------------
-   Fixed bugs with externals wordlists
-   Added 80018 subdomains

v3.4.47-rc Gained more Power! (05.07.2017)
------------------------------------------
- Added IPs lookup for subdomain scans
- Added missing HTTP statuses
- Bugfix: encoding errors (supported cp1251,utf8,utf16) for body analyze
- Bugfix: allow to use both --random-list & --extension params
- Directory closing slash has been removed
- Support Internationalized Domain Names IDNA
- Removed --indexof (-i) params
- Add --ignore-extensions -i param to ignore a selected extension
- Added --sniff param to process responses
    - indexof   (detect Apache Index Of/ directories)
    - file      (detect large files)
    - collation (heuristic detect invalid web pages)
    - skipempty (skip empty valid pages)
- Internal dictionaries have been filtered out. Delete all duplicates
- Added +990 unique directories (36931)

v3.3.37-rc (22.06.2017)
------------------------
- Fixed errors
- Add config wizard (allows you to configure an own project)
    
v3.2.36-rc (04.06.2017)
------------------------
- Added custom reports directory --reports-dir /home/user/Reports
- Added user guide --docs
- Reusable proxy requests pooling in --tor, --torlist
- Prevent socks5 proxy warnings
- Optimizing scan execution
- Request delays allow using of milliseconds
- Python2.7 no longer support

v3.1.32-rc (02.06.2017)
------------------------
- Add extensions filter --extensions php,json etc

v3.0.32-rc (19.05.2017)
-----------------------
- Add global installation

v3.0.31-rc (20.02.2017)
------------------------
- update directories
- fixes for redirects

v3.0.3-rc (17.02.2017)
-----------------------
- fixes for https stuff scan
- cleared internal wordlists
- increased coverage
    
v3.0.3-beta (13.02.2017)
-------------------------
- detect SSL cert requires
- added 7150 directories
- fixes for https subdomains
- more unit coverages
    
v3.0.2-beta (31.01.2017)
------------------------
- relieved of unnecessary dependencies
- fully optimized code inside
- user-friendly interface
- multiple reporters (std,txt,json,html)
- added external wordlists support
- added external proxylist support
- added wordlist shuffling
- wordlist prefixes
- added multithreading control
- dynamic and smart requests (cookies + accept headers)
- apache index of/ and files detection

v2.7.96  - v1.0.0 (05.01.2017)
------------------------------

* *v1.0.0* - all the basic functionality is available
* *v1.0.1* - added debug level as param --debug
* *v1.2.1* - added filesystem logger (param --log)
* *v1.2.2* - added example of usage (param --examples)
* *v1.3.2* - added possibility to use random proxy from proxylist (param --proxy)
* *v1.3.3* - simplify dependency installation
* *v1.3.4* - added code quality watcher
* *v1.3.5* - added ReadTimeoutError ProxyError handlers
* *v1.3.51* - fixed code style, resolve file read errors
* *v1.3.52* - code doc style added
* *v2.3.52* - subdomains scan available! (param --check subdomains). Added databases
* *v2.3.54* - disabled treads error. Refactored
* *v2.4.62* - change port is available now! (param --port 8080). Code style fixes
* *v2.5.62* - HTTPS support added
* *v2.6.62* - added 19000 Possible directories!
* *v2.7.62* - added redirect handler (Beta)
* *v2.7.72* - added 52 directories, small changes for UI
* *v2.7.82* - added 683 directories
* *v2.7.92* - exclusion list added Data/exclusions.dat
* *v2.7.95* - large files definitions , bad requests detection handler
* *v2.7.96* - optimize debug levels (0 - 1 - 2 param --debug) , optimize imports