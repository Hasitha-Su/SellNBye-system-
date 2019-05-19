# SellNBye-system-

This project is completed using node js and mongodb. 
open the project with a  suitable IDE and in termina use command "npm install" and then npm start
database connection will be established.
now postman or suitable tool can be used for api requesting

following is api documentation for each function

clickable link if necessary

https://drive.google.com/open?id=17iY2ISEtAn0o_POLnMq4w56N_uE4UBix

API Documentation

Buyer :
Insert:
URL: localhost:3000/api/buyer/
Method: POST
Sample Body: {
    "name" : "Daniel",
    "email" :"daniel@gmail.com",
    "location" : "England",
    "reputation" : 5,
    "username":"daniel123",
    "userId": 1
}

View
URL: localhost:3000/api/buyer/
Method: GET
Update
URL: localhost:3000/api/buyer/1
Method: PUT
Sample Body:{
    "name" : "Daniel",
    "email" :"dan@gmail.com",
    "location" : "England",
    "reputation" : 5,
    "username":"daniel123",
    "userId": 1
}
Delete
URL: localhost:3000/api/buyer/1
Method: DELETE
Seller
Insert
URL:localhost:3000/api/seller/
Method: POST
Sample Body: {
    "name" : "Daniel",
    "email" :"daniel@gmail.com",
    "location" : "England",
    "reputation" : 5,
    "username":"daniel123",
    "userId": 1
}
View
URL: localhost:3000/api/seller/
Method: GET
Update
URL: localhost:3000/api/seller/1
Method: PUT
Sample Body:{
    "name" : "Daniel",
    "email" :"dan@gmail.com",
    "location" : "AUS",
    "reputation" : 5,
    "username":"daniel123",
    "userId": 1
}
Delete
URL: localhost:3000/api/seller/1
Method: DELETE





Cart
Insert
URL:localhost:3000/api/cart/
Method: POST
Sample Body: {
    "cartId": 1,
    "items": [
        {
            "itemId": 1,
            "quantity": 10
        },
        {
            "itemId": 2,
            "quantity": 5
        }
    ],
    "buyerId": 1,
    "currentAmount": 200,
    "expireDate": "2019/05/19"
}
View
URL: localhost:3000/api/cart/1
Method: GET
Update
URL: localhost:3000/api/cart/1
Method: PUT
Sample Body:{
    "cartId": 1,
    "items": [
        {
            "itemId": 1,
            "quantity": 20
        },
        {
            "itemId": 2,
            "quantity": 5
        }
    ],
    "buyerId": 1,
    "currentAmount": 200,
    "expireDate": "2019/05/19"
}
Delete
URL: localhost:3000/api/cart/1
Method: DELETE


Item
Insert
URL:localhost:3000/api/item
Method: POST
Sample Body:{
    "name": "Watch",
    "itemId": 1,
    "description": "Test Desc",
    "unitPrice": 50,
    "sellerId": 1,
    "quantity": 10
}
View
URL: localhost:3000/api/item/
Method: GET
Update
URL: localhost:3000/api/item/1
Method: PUT
Sample Body:{
    "name": "Watch",
    "itemId": 1,
    "description": "Test Desc",
    "unitPrice": 70,
    "sellerId": 1,
    "quantity": 10
}
Delete
URL: localhost:3000/api/item/1
Method: DELETE

FeedBack
Insert
URL:localhost:3000/api/feedback
Method: POST
Sample Body:{
    "feedBackId": 1,
    "message": "Test feedback",
    "itemId": 1,
    "buyerId": 2,
    "rating": 4.5
}

View
URL: localhost:3000/api/feedback/
Method: GET
Update
URL: localhost:3000/api/feedback/1
Method: PUT
Sample Body:{
   "feedBackId": 1,
    "message": "Test feedback edited",
    "itemId": 1,
    "buyerId": 2,
    "rating": 4.5
}


Delete
URL: localhost:3000/api/feedback/1
Method: DELETE
