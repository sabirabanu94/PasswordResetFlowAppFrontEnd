# Password Reset Flow App - Front End - Guvi Zen Mainboot Task

This is a FrontEnd repo consists Password Reset Flow App Using Node JS [MERN].

## Netlify Deployment URL

I have attached the link for the Base URL of the Deployment. Along with the link use routes to test various pages.
[FrontEnd](https://passwordresetflowapp.netlify.app/)

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup and Installation](#setup-and-installation)
- [Routes](#Route-Values)
- [Deployment](#deployment)

## Features
- **User Registration Form**: Register new users with hashed passwords. 
- **User Login Form**: Authenticate users and issue JWTs for authorized access. These were done by Backend.
- **JWT-Based Authorization**: Protect routes using httpOnly tokens.
- **Secure User Info Retrieval**: Users can retrieve their information using valid tokens.
- **Error Handling and Validation**: Proper error messages and input validations.
- **Route Documentation**: Detailed documentation using Postman, with sample requests and responses.

## Tech Stack
- **ReactJS**: JavaScript library for Front End Application.
- **Tailwind CSS**: FrontEnd Styling Technology.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/yourrepository.git
   cd yourrepository

2. Install dependencies:
    ```bash 
    npm run build
3. Run the Application
    ```bash
        npm run dev

## Routes
    baseURL:https://passwordresetflowapp.netlify.app/
1. [Home Route](https://passwordresetflowapp.netlify.app/) `('/')`-> **Home URL**
2. [Login Route](https://passwordresetflowapp.netlify.app/signin) `('/signin')`-> **Login URL**
3. [Registration Route](https://passwordresetflowapp.netlify.app/register) `('/register')`-> **Registration URL**
4. [Forget Password Route](https://passwordresetflowapp.netlify.app/PasswordReset) `('/PasswordReset')`-> **Forget Password URL**
4. [UserInfo Route](https://passwordresetflowapp.netlify.app/userInfo) `('/userInfo')`-> **Get User Information URL** - This is a protected route. It works only when the user is logged in.

> [!NOTE]
> The Routes ***Home***,***Login***,***Registration*** and ***Forget Password Route*** are public routes. The Only protected route is ***UserInfo Route***.

> [!NOTE]
> We generate Emails after the successful registration of the user. The application emails the credentials to the user.
> Incase if the user forgot their password, using the email, we forward them the tokens which will be valid for 3 Hours. Within that three hours, they can use the token to reset their password for the application. Unless it will invalid.


## Deployment

The application can be deployed to Netlify for public access.

1. Pushed the code to GitHub.
2. Deployed the application by connecting our GitHub repository to Netlify App.
3. Use the [Netlify URL](https://passwordresetflowapp.netlify.app/) to access our deployed Application.


