# Usage

To use the credentials file aws_creds.yml, you can use the --extra-vars
option to include them in the current playbook run.

``` shell 
ansible-playbook ./create-rds-db.yaml --extra-vars=@~/aws_creds.yml 
```
