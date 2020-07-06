## This repository contains the source code for the medium blog titled : 'Creating RESTful API's in Django Rest Framework using Class-Based Views'

You can find the blog here : 

#### Landing page
```
HTTP 200 OK
Allow: GET, HEAD, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "message": "Welcome",
    "documentation": "<specify notes>"
}
```
#### GET Request
GET /sports
```
HTTP 200 OK
Allow: GET, POST, HEAD, OPTIONS
Content-Type: application/json
Vary: Accept

[
    {
        "id": 1,
        "name": "MS Dhoni",
        "sport": "Cricket",
        "age": 38
    },
    {
        "id": 4,
        "name": "Cristiano Ronaldo",
        "sport": "Football",
        "age": 35
    }
]
```

#### POST Request
POST /sports
```
{
        "name": "Virat Kohli",
        "sport": "Cricket",
        "age": 31
}
```

RESPONSE 
```
HTTP 201 Created
Allow: GET, POST, HEAD, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "id": 7,
    "name": "Virat Kohli",
    "sport": "Cricket",
    "age": 31
}
```

#### PUT Request
PUT /sports/<id>
```
  {
    "name": "Rohit Sharma",
    "sport": "Cricket",
    "age": 31
  }
```
  
RESPONSE
```
HTTP 200 OK
Allow: GET, PUT, DELETE, HEAD, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "id": 7,
    "name": "Rohit Sharma",
    "sport": "Cricket",
    "age": 31
}
```

#### DELETE Request
DELETE /sports/<id>

RESPONSE
```
{
    "id": null,
    "name": "Rohit Sharma",
    "sport": "Cricket",
    "age": 31
}
```
  
