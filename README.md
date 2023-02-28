#### Base environment
- install vscode & extenstion
    - REST Client
    - Thuder Client
    - Path Intellisense
    - Prettier - Code formatter
    - vscode-icons
    - vue-format
    - Go
    - Drawio Preview
    - Draw.io Integration: Mermaid plugin

- install git Desktop
```
    url :
```
- install Docker desktop 
```
    url :
```
### set desktop for dev
#### git clone environment for dev local
```
    git clone http://github.com/gmmoshopping/environment

    cd environment
    
```
#### git clone go 
```
    git clone http://github.com/gmmoshopping/gomaster
```

### set environment for dev in local 
##### run service for base environment
```
docker-compose -f docker-compose.yml up -d
```

##### stop service for base environment
```
docker-compose -f docker-compose.yml down
```
##### run service store
```
docker-compose -f docker-compose-storage.yml up -d
```

##### down service stop store 

```
docker-compose -f docker-compose-storage.yml down
```
#### run api gateway
#### run service ngix manger rever proxy 
```
docker-compose -f docker-compose-ngix.yml up -d 
```

#### run service ngix manger rever proxy 
```
docker-compose -f docker-compose-ngix.yml down
```
##### Log in to the Admin UI
-   When your docker container is running, connect to it on port 81 for the admin interface. Sometimes this can take a little bit because of the entropy of keys.
```
http://127.0.0.1:81
```
Default Admin User:
```
Email:    admin@example.com
Password: changeme
```
-   Immediately after logging in with this default user you will be asked to modify your details and change your password.

