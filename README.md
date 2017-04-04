# Linux-Server-Configuration
Linux Server Configuration study project

#### Notes to reviewer:
* IP address: 159.203.124.46
* SSH port: 2200
* Full SSH-connection string: ` ssh grader@159.203.124.46 -p 2200 `
* Complete url to Catalog application: ` http://server-conf-project.tk `
  * App is also accessable by server's ip address, but this kind of connection is not advisable because of Google's restrictions to use the public ip as a return address after user authorization(` http://stackoverflow.com/questions/14238665/can-a-public-ip-address-be-used-as-google-oauth-redirect-uri `).
* Installed software:
  * Apache web server (`apache2`)
  * Postgresql database engine (`postgres`)
  * WSGI module (`libapache2-mod-wsgi `)
  * Flask library (` python-flask `)
  * SQLAlchemy library (` python-sqlalchemy `)
  * Google OAuth library (` python-oauth2client `)
  
* Configuration changes made:
  * 
