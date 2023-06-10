# A REST API With JSON Server for testing

https://my-json-server.typicode.com/vldi2000/jsonserver

The following HTTP endpoints are created automatically by JSON server: 

https://my-json-server.typicode.com/vldi2000/jsonserver/employees
* GET    /employees
* GET    /employees/{id}
* POST   /employees
* PUT    /employees/{id}
* PATCH  /employees/{id}
* DELETE /employees/{id}

Code example using python requests below:

GET   /employees
```
import requests

url = "https://my-json-server.typicode.com/vldi2000/jsonserver/employees"

payload = ""
headers = {"Content-Type": "text/plain"}

response = requests.request("GET", url, data=payload, headers=headers)

print(response.text)
```

POST   /employees 
```
import requests

url = "https://my-json-server.typicode.com/vldi2000/jsonserver/employees"

payload = {
    "id": 4,
    "first_name": "James",
    "last_name": "Holler",
    "email": "james@codingthesmartway.com"
}
headers = {"Content-Type": "application/json"}

response = requests.request("POST", url, json=payload, headers=headers)

print(response.text)
```
