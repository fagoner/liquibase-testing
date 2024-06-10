# liquibase-testing
Testing liquibase in ubuntu (22.04)



### Installing on ubuntu 22.04

Open a terminal 

```
wget -O- https://repo.liquibase.com/liquibase.asc | gpg --dearmor > liquibase-keyring.gpg && \
cat liquibase-keyring.gpg | sudo tee /usr/share/keyrings/liquibase-keyring.gpg > /dev/null && \
echo 'deb [arch=amd64 signed-by=/usr/share/keyrings/liquibase-keyring.gpg] https://repo.liquibase.com stable main' | sudo tee /etc/apt/sources.list.d/liquibase.list
```

Update the package lists:
`sudo apt-get update`

Install Liquibase:
`sudo apt-get install liquibase`

Ensure that Liquibase is updated to the desired version:
`liquibase --version`

