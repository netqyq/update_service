# Update Service

update_server's script is use for to update your service, 

## Using Case
for example,you hava a search service , the dir stacture is:
```
    /data/search/
            bin/search
            data/*.data
            log/*.log
```

and you should define the configuration section like :
```
# data_dir_name is the data dir name that you want to update
data_dir_name=data

# src is the new data's dir, wait to be use.
src=/data/update/0403

# dst is destination dir of the data's home
dst=/data/search/

# svr_home is the home dir of the service
svr_home=/data/search

# bin_name is the name of bin file(the service)
bin_name=search

# start is to start the service,you must have a start script for start the service located at the $svr_home
start=./start

# stop is to stop the service,you must have a stop script for stop the service located at the $svr_home
stop=./stop
                
```

the second script is use for to update your service(bin file)

for example:
  you hava a xserver service , the dir stacture is:
    /data/server/xserver
            bin/xsd
            log/*.log






              
