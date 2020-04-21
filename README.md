### Prerequisites

What things you need to install the software and how to install them

```
node
npm/yarn
mongodb

```

### Pre-set Steps

Create a `.env` file in the root folder where package.json file exists

in that file copy and paste the below code

```
PORT=4200
MONGODB_URL=mongodb://localhost:27017
JWT_KEY=harsha_first
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
npm install/yarn install

```


## Running the application

```
npm start/yarn start
```

### Usage

* users/ - POST 

To signup

```
header: application/json
payload:
{
    "name":"<name>",
    "email":"<email>",
    "password":"<password>"
}
```

* users/login - POST 

To Login

```
header: application/json
payload:
{
    "email":"<email>",
    "password":"<password>"
}
```

* users/me - GET 

To get the login user details

```
Authorization : Bearer <token>(which given in login response)
```

* users/logout - POST 

To logout

```
Authorization : Bearer <token>(which given in login response)
```

* users/logoutall - POST 

To logout from all places

```
Authorization : Bearer <token>(which given in login response)
```
