# rest-client-example

### LOGIN
POST http://localhost:3000/login HTTP/1.1
Content-Type: application/json

{
    "username":"18500290402",
    "password":"888888"
}

### EXTEND
PATCH http://localhost:3000/login HTTP/1.1
Content-Type: application/json
Refresh: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJyZWZyZXNoIjp0cnVlLCJ0b2tlbklkIjoiVE9NRC12Q0dUZHBYdy1aa29QYS1TdnVtUyIsInVzZXJJZCI6IlVTWE5OTUNWT0pTUiIsImlhdCI6MTYwOTIyNTY0NCwiZXhwIjoxNjExODE3NjQ0fQ.zEnXLa4OWmwR55TyvCAqWEd4u-5DPB5tUiMqfpA3xF0

### PUBLIC KEY
GET http://localhost:3000/pubkey HTTP/1.1

### LOGOUT
### BLOCK
### DISABLE
### DEACTIVATE

### START EMAIL CONFIRMATION
### END EMAIL CONFIRMATION
### START PASSWORD RECOVERY
### END PASSWORD RECOVERY
### UPDATE PASSWORD

### GET USERS
GET http://localhost:3000/users HTTP/1.1

### CREATE USER
POST http://localhost:3000/users HTTP/1.1
Content-Type: application/json

{
    "username":"15643638289",
    "email":"max@me.com",
    "password":"999999"
}

### GET USER
GET http://localhost:3000/users/1 HTTP/1.1
### EDIT USER
PATCH http://localhost:3000/users/9 HTTP/1.1
Content-Type: application/json

{
    "email":"delta@me.com",
    "password":"888888"
}
### DELETE USER
DELETE http://localhost:3000/users/9 HTTP/1.1
### UPDATE USER ROLES
PATCH http://localhost:3000/users/1/roles HTTP/1.1
Content-Type: application/json

{
    "roleId": [1,2]
}

### GET ROLES
GET http://localhost:3000/roles HTTP/1.1
### CREATE ROLE
POST http://localhost:3000/roles HTTP/1.1
Content-Type: application/json

{
    "name": "fantas",
    "description": "teachers priveliges"
}
### GET ROLE
GET http://localhost:3000/roles/1 HTTP/1.1
### EDIT ROLE
PATCH http://localhost:3000/roles/1 HTTP/1.1
Content-Type: application/json

{
    "name":"admin",
    "description":"complete access to all systems"
}
### DELETE ROLE
DELETE http://localhost:3000/roles/1 HTTP/1.1
### UPDATE ROLE USERS
PATCH http://localhost:3000/roles/1/users HTTP/1.1
Content-Type: application/json

{
    "roleId": [1]
}
