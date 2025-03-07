sequenceDiagram  
participant browser
participant server

browser -->> server: POST https://https://studies.cs.helsinki.fi/exampleapp/new_note
activate server
server -->> browser : URL Redirection
deactivate server
browser -->> server: GET https://https://studies.cs.helsinki.fi/exampleapp/new_note
activate server
server -->> browser: The html file
deactivate server
browser -->> server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
activate server
server -->> browser: The css file
deactivate server
browser -->> server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
activate server
server -->> browser: The js file
deactivate server
browser -->> server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
activate server
server -->> browser: The css file
deactivate server
browser -->> server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
activate server
server -->> browser: The json file
deactivate server
browser -->> server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
activate server
server -->> browser: The css file
deactivate server
browser -->> server: GET https://studies.cs.helsinki.fi/exampleapp/favicon.ico
 activate server
server -->> browser: The favicon file
deactivate server
