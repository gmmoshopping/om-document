#### Base environment
- install vscode & extenstion
    - [Download & install](https://code.visualstudio.com)
    - [REST Client url](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
    - [Thuder Client url](https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client)
    - [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
    - [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    - [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
    - [vue-format](https://marketplace.visualstudio.com/items?itemName=febean.vue-format)
    - [Go](https://marketplace.visualstudio.com/items?itemName=golang.Go)
    - [vscode-go-syntax](https://marketplace.visualstudio.com/items?itemName=dunstontc.vscode-go-syntax)
    - [Drawio Preview](https://marketplace.visualstudio.com/items?itemName=purocean.drawio-preview)
    - [Draw.io Integration: Mermaid plugin](https://marketplace.visualstudio.com/items?itemName=nopeslide.vscode-drawio-plugin-mermaid)

- install git Desktop
    - [Download & install Git Desktop](https://desktop.github.com)
    - [Download & install Git](https://git-scm.com/download/win)
- install Docker desktop 
    - [Download & install](https://www.docker.com/products/docker-desktop/)

## Setting up the development environment 
#### git clone environment for dev local
```
    git clone http://github.com/gmmoshopping/environment

    cd environment
    
```
#### git clone go boilerplate for start coding
```
    git clone https://gitlab.com/osp-cs/order-management/golang-api-boilerplate.git
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

