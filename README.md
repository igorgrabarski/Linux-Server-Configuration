# Linux-Server-Configuration
Linux Server Configuration study project

#### Notes to reviewer:
* IP address: 159.203.124.46
* SSH port: 2200
* Full SSH-connection string: ` ssh grader@159.203.124.46 -p 2200 `
* Complete url to Catalog application: ` http://server-conf-project.tk `
  * App is also accessable by server's ip address, but this kind of connection is not advisable because of Google's               restrictions to use the public ip as a return address after user authorization(`                                     http://stackoverflow.com/questions/14238665/can-a-public-ip-address-be-used-as-google-oauth-redirect-uri `)
* Installed software:
    * Apache web server (`apache2`)
    * Postgresql database engine (`postgres`)
    * WSGI module (`libapache2-mod-wsgi `)
    * Flask library (` python-flask `)
    * SQLAlchemy library (` python-sqlalchemy `)
    * Google OAuth library (` python-oauth2client `)
    * Package list updated
    * Installed packages upgraded
  
* Configuration changes made:
  * New user creation with name ` grader `
  * Adding this user to ` sudoers ` configuration to allow using of ` sudo ` command
  * Generating of rsa-key for more secured ssh connection
  * Key-based SSH authentication configuring
  * Restriction to log in as root remotely configured
  * SSH port set to 2200
  * Firewall(ufw) configured to allow only incoming connections on ports 2200, 80 and 123
  * Web server(Apache) is configured to respond on port 80 (both by ip address and domain name)
     * Note: Please do not use ` www ` prefix as it is not available on this free of charge domain name.
  * PostgreSQL database server was configured to run on this host. User ` grader ` with the same password has been created         Application ` Catalog App  ` utilizes the database named ` catalog ` that has also been created
  * Appropriate file ` Catalog.conf  ` has been created and configured in dir ` /etc/apache2/sites-available `
  
