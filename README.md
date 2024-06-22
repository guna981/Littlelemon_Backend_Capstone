# Little Lemon Backend

> LittleLemon app developed using Django for the Back-End Developer Capstone course offered by Meta. This Capstone project enables you to demonstrate multiple skills by solving an authentic real-world problem. The project aims to test your abilities in full-stack back-end development in a real-life scenario by composing a Django web app. Each module includes a brief recap of, and links to, content that you have covered in previous courses in this program.

> Little Lemon Backend is a robust Django backend designed to power the Little Lemon app, the API offers endpoints for managing customers, menu items, categories, orders, delivery crew users and user groups.


## Project Requirements

- Users should be able to register, login and logout
- Customers should be able to browse menu items and categories, add items to cart, clear their cart, make orders
- Managers should be able to fully manage categories and menu items, they can also update orders, assign delivery crew orders and assign customers a group
- Delivery crew users should be able to update their assigned orders



## Endpoints

### User Authentication Endpoints

| Endpoint                | Role                            | Method | Purpose                                                                    |
| ----------------------- | ------------------------------- | ------ | -------------------------------------------------------------------------- |
| /api/auth/register      | No role required                | POST   | Registers a new user and returns 201 - Created HTTP status code            |
| /api/auth/profile       | Anyone with a valid user token  | POST   | Displays only the current user                                             |
| /api/auth/token/refresh | Anyone with valid refresh token | POST   | Generates access token that can be used in other API calls in this project |
| /api/auth/logout        | Logs the user out               | POST   | Generates access token that can be used in other API calls in this project |

##### Following are the API URL

http://127.0.0.1:8000/restaurant/menu/       
http://127.0.0.1:8000/restaurant/menu/2/     
http://127.0.0.1:8000/restaurant/api-token-auth/ (POST METHOD)
http://127.0.0.1:8000/restaurant/booking/ 



##### Djoser:
http://127.0.0.1:8000/auth/users/   
http://127.0.0.1:8000/auth/users/me/
http://127.0.0.1:8000/auth/users/confirm/
http://127.0.0.1:8000/auth/users/resend_activation/
http://127.0.0.1:8000/auth/users/set_password/
http://127.0.0.1:8000/auth/users/reset_password/
http://127.0.0.1:8000/auth/users/reset_password_confirm/
http://127.0.0.1:8000/auth/users/set_username/
http://127.0.0.1:8000/auth/users/reset_username/
http://127.0.0.1:8000/auth/users/reset_username_confirm/

##### Djoser TOKEN:
http://127.0.0.1:8000/auth/token/login/

