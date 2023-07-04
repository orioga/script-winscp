# script-winscp
Script for publishing folders and files


# Some basic commands are:
### Connect
```
open sftp://root:mypassword@sftp.cloud.web.it/
```

### Option
```
#Connection option
option batch continue
option confirm off
```

### Delete
```
rm		/var/www/vhosts/service.com/httpdocs/update/OldFiles/file.xml
rmdir   /var/www/vhosts/service.com/httpdocs/update/OldFiles/directory
```

### deploy
```
put \\service\directory\		/var/www/vhosts/service.com/httpdocs/update/NewFiles/*
put \\service\file.xml	    /var/www/vhosts/service.com/httpdocs/update/NewFiles/*
```

### move
```
mv /var/www/vhosts/service.com/httpdocs/update/NewFiles/directory		/var/www/vhosts/service.com/httpdocs/update/directory
mv /var/www/vhosts/service.com/httpdocs/update/NewFiles/file.xml	/var/www/vhosts/service.com/httpdocs/update/file.xml
```

# Disconnect
```
close
```
