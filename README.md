# Error-when-pip-install
ERROR:
>pip install pods

ERROR: No matching distribution found for pods
WARNING: pip is configured with locations that require TLS/SSL, however the ssl module in Python is not available.
Could not fetch URL https://pypi.org/simple/pip/: There was a problem confirming the ssl certificate: HTTPSConnectionPool(host='pypi.org', port=443): Max retries exceeded with url: /simple/pip/ (Caused by SSLError("Can't connect to HTTPS URL because the SSL module is not available.")) - skipping

solution: use image to accelarate(such as douban)
the new command:
pip install [package name] -i http://pypi.douban.com/simple/ --trusted-host pypi.douban.com
