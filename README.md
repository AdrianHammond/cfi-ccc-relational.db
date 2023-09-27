#AWS Set up

AWS requires a default VPC to be created
AWS requires a default Subnet to be created


# Usage

To use the credentials file aws_creds.yml, you can use the --extra-vars
option to include them in the current playbook run.

``` shell 
ansible-playbook ./create-rds-db.yaml --extra-vars=@~/aws_creds.yml 
```

The variables can also be passed directly from the command line 

``` shell 
ansible-playbook ./create-rds-db.yaml --extra-vars “AWS_ACCESS_KEY_ID=MYACCESSKEY AWS_SECRET_ACCESS_KEY=MYSECRETACCESSKEY RDS_DB_USERNAME=cfiuser RDS_DB_PASSWORD=cfi#12345"
```

