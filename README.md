#meo-wifi-login

## Description:
Allows for an automated login through a MEO Wifi Premium hotspot.

## Usage
You may use 'meo_wifi_login.py' file as regular script, running it via CLI...:

```
./meo_wifi_login -u <username> -p <password>
```

...or call the 'meo_wifi_login' function through your script:
```
import meo_wifi_login

meo_wifi_login.meo_wifi_login('user','pass')
```

The script also looks for a 'MEO_WIFI_USER' and 'MEO_WIFI_PASSWORD' environment variable for the login information.

In case neither of these sources are available, it will prompt the user via console to fill them


## Required Python libraries
Beyond the standard Python libraries, you need the 'requests' library.

You can install it using pip:

```
pip install requests 
```

Several Linux distros also have a package for it. For example, in Ubuntu 12.04 you can:

```
sudo apt-get install python-requests
```

Python earlier than 2.7.9 have restrictions in their ssl module that limit the configuration that urllib3 can apply.

If you have a `InsecurePlatformWarning` error, update Python to 2.7.9+ or install requests extra packpage:


```
pip install requests[security]
```

This installs following extra packages:

pyOpenSSL<br>
ndg-httpsclient<br>
pyasn1








