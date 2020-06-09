# 329-Azure API Management with Logic App

This example tries to illustrate how you can create
example API to your APIM using Logic App. 

This ARM template implementation follows **feature** folder structure
meaning that each API has it's own folder and all resources
related to that API in that folder. 

E.g. All content of api _users_ is in `api/users` folder:

```cmd
.
├───api
│   └───users
└───policies
```

That folder has following files:

```cmd
api.json
api-get.xml
logicapp.json
```

`api.json` is ARM template of the users API.

`api-get.xml` is APIM policy for GET method.

`logicapp.json` is ARM template for the backend API implemented as Logic App.
