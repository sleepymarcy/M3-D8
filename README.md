# M3-D8
Building the new Amazon



CRUD endpoint
https://striveschool-api.herokuapp.com/api/product/

The product model is 
{
    "_id": "5d318e1a8541744830bef139", //SERVER GENERATED
    "name": "app test 1",  //REQUIRED
    "description": "somthing longer", //REQUIRED
    "brand": "nokia", //REQUIRED
    "imageUrl": "https://drop.ndtv.com/TECH/product_database/images/2152017124957PM_635_nokia_3310.jpeg?downsize=*:420&output-quality=80", //REQUIRED
    "price": 100, //REQUIRED
    "userId": "admin", //SERVER GENERATED
    "createdAt": "2019-07-19T09:32:10.535Z", //SERVER GENERATED
    "updatedAt": "2019-07-19T09:32:10.535Z", //SERVER GENERATED
    "__v": 0 //SERVER GENERATED
}

#---------------------------------------------------------------#
EVERY REST API CALL SHOULD BE AUTHENTICATED. 
Every request to the API should use Token Based Authentication to secure access to the contents.
You can get your token by registering on: strive.school/studentlogin
Authorization: Bearer ###########
Where ######### is the access_token returned by the endpoint.
#---------------------------------------------------------------#
Today you have to implement:
- A backoffice page, where you can insert the product by specifying the parameters
- A front page, where the user can see the available products
------ N.B. ------
Tokens duration is set to 14 days. Whenever you'll need to obtain a new one you can send the following request:

POST https://striveschool-api.herokuapp.com/api/account/login
{
    "username": "testusername@yourmail.com",
    "password":"pass"
}