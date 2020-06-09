# 329-Azure API Management with Logic App

This example tries to illustrate how you can create
example API to your APIM using Logic App. 
Here the overview of the deployment:

![Azure API Management deployment overview](https://user-images.githubusercontent.com/2357647/84140538-754d4c00-aa5a-11ea-9bfd-afe1a775f313.png)

This ARM template implementation follows **feature** folder structure
meaning that each API has it's own folder and all resources
related to that API in that folder. 

E.g. All content of api _users_ is in `api/users` folder:

```cmd
/
├───api
│   ├───products
│   └───users
└───policies
```

That folder has following files:

```cmd
api.json
api-post.xml
logicapp.json
```

`api.json` is ARM template of the users API.

`api-post.xml` is APIM policy for POST method.

`logicapp.json` is ARM template for the backend API implemented as Logic App.

Similarly for `products` there is just one additional file for OpenAPI spec:

`products.yaml` OpenAPI spec for products API.
