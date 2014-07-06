# php-oauth + simpleSAMLphp + app/api server + client application #
The goal of this project is to implement the [php-oauth](https://github.com/fkooman/php-oauth) OAuth 2.0
authorization server along with simpleSAMLphp and example applications that implement and consume APIs
using OAuth 2.0.

## Installation / Setup ##
This project uses Vagrant with VirtualBox to setup local servers and install the needed software. All you need
to do to test this out is:

1. Clone this repo
2. From the command line, go to the vagrant folder in the repo
3. Add the following entries to your hosts file
4. Run ```vagrant up```
5. Once vagrant is done spinning up the three virtual machines, open your browser and go to
[http://appclient.local/](http://appclient.local/)
6. You should see a simple page, click the Login link in the header and you should be redirected to login and grant
access.
7. Login with username ```user1``` and password ```pass1```.
8. After being logged in you'll see a sort of debug page showing the output of a few API calls being made
to the appserver.local host.


    # /etc/hosts
    # OAuth POC hosts
    192.168.55.10 saml.local
    192.168.55.11 oauth.local
    192.168.55.12 demo.local appserver.local appclient.local