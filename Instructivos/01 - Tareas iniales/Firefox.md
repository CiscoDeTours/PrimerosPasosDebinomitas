# Firefox

#### I.1 - Add the Mozilla repo for a up to date browser

~~~
sudo install -d -m 0755 /etc/apt/keyrings
~~~

~~~
wget -q https://packages.mozilla.org/apt/repo-signing-key.gpg -O- | sudo tee /etc/apt/keyrings/packages.mozilla.org.asc > /dev/null
~~~

~~~
echo "deb [signed-by=/etc/apt/keyrings/packages.mozilla.org.asc] https://packages.mozilla.org/apt mozilla main" | sudo tee -a /etc/apt/sources.list.d/mozilla.list > /dev/null
~~~

~~~
echo '
Package: *
Pin: origin packages.mozilla.org
Pin-Priority: 1000
' | sudo tee /etc/apt/preferences.d/mozilla 
~~~

~~~
sudo apt update
~~~

~~~
sudo apt install firefox
~~~


#### I.2 - Uninstall the ESR version

~~~
sudo apt remove firefox-esr
~~~


#### I.3 - Webapps capability

• Add the project repo:

~~~
curl -fsSL https://packagecloud.io/filips/FirefoxPWA/gpgkey | gpg --dearmor | sudo tee /usr/share/keyrings/firefoxpwa-keyring.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/firefoxpwa-keyring.gpg] https://packagecloud.io/filips/FirefoxPWA/any any main" | sudo tee /etc/apt/sources.list.d/firefoxpwa.list > /dev/null
~~~

~~~
sudo apt update
~~~

~~~
sudo apt install firefoxpwa
~~~

• Install the extension:

https://addons.mozilla.org/es-ES/firefox/addon/pwas-for-firefox/

• Install the runtime:


#### I.4 - Language packages

• Search for aditional languages:

~~~
sudo apt search firefox-l10n
~~~

• Install your native language:

~~~
sudo apt install firefox-l10n-es-es
~~~
