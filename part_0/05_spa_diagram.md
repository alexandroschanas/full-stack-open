```mermaid
sequenceDiagram
participant browser
participant server

browser -->> server : GET https://studies.cs.helsinki.fi/exampleapp/spa
activate server
server -->> browser : 200 OK , Redirection
deactivate server

browser -->> server : GET https://studies.cs.helsinki.fi/exampleapp/spa/main.css
activate server
server -->> browser : 200 OK , Get css file
deactivate server

browser -->> server : GET https://studies.cs.helsinki.fi/exampleapp/spa/spa/js
activate server
server -->> browser : 200 OK , Get js file
deactivate server

browser -->> server : GET https://studies.cs.helsinki.fi/exampleapp/data.json
activate server
server -->> browser : 200 OK , Get json file
deactivate server
```
