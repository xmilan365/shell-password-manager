# shell_password_manager
Create and check passwords using terminal by running shell scripts.

# create_pass
create_pass shell script will create randomly generated password based on input parameters:
-h, --help 	 display this help and exit
-l, --lowercase  include lowercase characters in the password
-u, --uppercase  include uppercase characters in the password
-n, --number 	 include uppercase characters in the password
-s, --symbol 	 include spesific symbols in the password
-d, --dlzka 	 specify lenght of the password, defaulty set to 12

User is asked to provide desired username and service for which will credentials be used and record is saved to database. In the end, user has option to send this record to his personal mail readed from config.sh file.

# check_pass
check_pass shell script will check passwords, username or service from database from terminal. User needs to provide parameters:
-h	display this help and exit
-s	checking record based on service name
-u	checking record based on username
-p	checking record based on password

User needs to provide data based on provided parameter (e.g. check_pass -s netflix). The result is sql query that return desired info.

Information about personal mail, oracle username, oracle password is readed from config.sh file.
