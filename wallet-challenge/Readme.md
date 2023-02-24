## BackEnd Developer Challenge #1
#### Title :
Wallet Challenge
#### Description: 
We are going to have a microservice to keep all data of the user wallet. We need to have two API to expose them to other microservices.
##### Get Balance API:
This API should return a ```JSON``` to show the current balance of a user. The parameter which is needed for this API is ```user_id``` and the output should be like the below sample:

**method:** GET

**uri :** ```/api/v1/balance/{user_id}```

**Response:**
```json
{
  "status_code": 200,
  "result" : "SUCCESS",
  "messages":[],
  "data" : {
    "balance":4000
    }
}
```
##### Add Money API:
This API should add money to the wallet of a user and at the end return the transaction reference number. The parameter which is needed for this API is ```user_id``` and ```amount``` and the output should be like the below sample:

**method:** POST

**uri :** ```/api/v1/wallet/add```

**Request Body:**
```json
{
  "user_id" : 1234,
  "amount" : 4000
}
```

**Response:** 
```json
{
  "status_code": 200,
  "result" : "SUCCESS",
  "messages":[],
  "data" : {
    "reference_id":12312312312
    }
}
```

**Please consider the below points:**

- Dockerize the project
- Use ```MySQL``` as a database to store your data
- We need to Save all transaction logs of user
- We need an API to show balance of each user
- We need an API to add money to wallet of user
- We need to have some necessary test cases (just 6 test cases to make sure you know
how to write test cases)
- We need a daily job to calculate total amount of transactions and print it on terminal
- You don’t have to develop any API or service for user, just develop the necessary
services which are related to wallet
