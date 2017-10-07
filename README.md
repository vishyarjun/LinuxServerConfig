# Linux Server Configuration

This project is a configuration of a Linux based Server created using Amazon Lightsail and deployment of Item Catalog Project in the server.

**Complete URL** : http://13.126.231.100/

**Public IP** : 13.126.231.100

**SSH Port** : 2200

## softwares installed
- **Apache**
- **mod-wsgi**
- **Python**
- **Flask**
- **SQLAlchemy**
-  **Request**
-  **httplib2**
-  **PostgreSQL**
-  **psycopg2**
-  **Git**
## Configuration changes made in server

 - Following Users are created

        -**ubuntu** - Sudo Access available

        -**grader** - Sudo Access available

        -**postgres** - Sudo Not available(created by Postgres)

 - Firewall is enabled
 - Incoming through Ports 2200,80,123,SSH only are enabled
 - Outgoing is enabled
 - New Postgres Database named Catalog is created
 - New DB user named catalog is created.
 - Time Zone of Server is in UTC
 - Item Catalog is deployed and Site is made available to run the flask application

## Grader login
`ssh grader@13.126.231.100 -p 2200 -i ~/.ssh/<your_rsa_dir>`
SSH Key available in `/home/grader/.ssh/authorized_keys`
Pass Phrase : grader123
The actual Key is available in the 'Notes to Reviewer' Field

### Pre-Requirements
1. Command Line/Terminal Installed to login server.

### Reference
1.  [Digital Ocean Flask Tutorial](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)
2. [stackoverflow](www.stackoverflow.com)
3. [Flask Documentation](http://flask.pocoo.org/docs/0.12/)
4. [Udacity Forum Discussion1](https://discussions.udacity.com/t/linux-server-configuration-500-internal-server-error/356689/22)
5. [Udacity Forum Discussion 2](https://discussions.udacity.com/t/deploy-item-catalog-in-linux-server/382099)
5. [PostgreSQL Documenation](https://www.postgresql.org/docs/)
