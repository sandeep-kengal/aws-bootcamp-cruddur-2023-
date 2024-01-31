# Week 3 — Decentralized Authentication

# Week 3 — Decentralized Authentication
This was technically the fourth week of the Bootcamp. 

(The Hyperlinks in the table below link to the training videos)
<hr/>

| Homework      | Completed     | Not Completed  |
| ------------- |:-------------:| -----:|
| [Decentralized Authentication](https://www.youtube.com/watch?v=9obl7rVgzJw&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=41)  | ✔     |    |
| [Ashish's - Decenteralized Authentication](https://www.youtube.com/watch?v=tEJIeII66pY&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=39)   | ✔ |  |
| [Setup Cognito User Pool](https://www.youtube.com/watch?v=9obl7rVgzJw&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=40)  | ✔     |    |
| [Implement Custom Signin Page](https://www.youtube.com/watch?v=9obl7rVgzJw&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=40) | ✔      |   |
| [Implement Custom Signup Page](https://www.youtube.com/watch?v=T4X4yIzejTc&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=41 )|✔      |   |
| [Watched Ashish's Week 2 - Observability Security Considerations](https://www.youtube.com/watch?v=bOf4ITxAcXc&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=31)|✔      |   |
| [Implement Custom Confirmation Page](https://www.youtube.com/watch?v=T4X4yIzejTc&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=41)|    ✔  |   |
| [Implement Custom Recovery Page](https://www.youtube.com/watch?v=T4X4yIzejTc&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=41)  | ✔   |   |
| [Different approaches to verifying JWTs](https://www.youtube.com/watch?v=nJjbI4BbasU&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=43) |✔      |   |
| [Cognito JWT Server side Verify](https://youtu.be/d079jccoG-M)| ✔   |   |
| [Improving UI Contrast and Implementing CSS Variables for Theming](https://youtu.be/m9V4SmJWoJU)| ✔   |  |

<hr/>

|    | Table of contents - Steps taken to complete Week 3 assignments                                                                                                                                                                         |
|----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | [Configuring and Installing AWS amplify](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#aws-amplify-install-in-env-vars)                                |
| 2  | [Importing AWS Amplify](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#aws-amplify-import-configuration)                                                |
| 3  | [Port startup configuration](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#updating-port-startup-public)                                               |
| 4  | [Cognito Backend fixes](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#updating-the-backend-aws-cognito-environment)                                    |
| 5  | [Submit Button fix](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#configuring-login-button-behaviour)                                                  |
| 6  | [Log in invalid user test](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#testing-the-log-in-button-behaviour-for-a-response)                           |
| 7  | [Test User creation](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito---setup-test-user-via-console)                                              |
| 8  | [Sign in options](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito---review-test-user-configuration-via-console)                                  |
| 9  | [Temporary password email sent](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito---username-and-password-sent-to-email)                                                     |
| 10 | [Required attributes](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito---setting-preferred-username-via-console)                                  |
| 11 | [Configure message delivery](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#user-confirmation-email)                                                    |
| 12 | [Userpool name](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#confirmed-users-account-status-changes-to-confirmed)                                     |
| 13 | [Advanced app client settings](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#userpool-creation)                                                        |
| 14 | [User attributes](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito---user-attributes)                                                             |
| 15 | [Final User pool](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito-user-pool-created)                                                             |
| 16 | [Force email confirmation in terminal](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito---confirming-email-via-terminal)                          |
| 17 | [Users account status changes to confirmed after responding to email](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#email-status-changed-to-confirmed) |
| 18 | [Userpool creation](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito-user-pool-dashboard)                                                         |
| 19 | [Cognito client ID](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#cognito-client-id)                                                                   |
| 20 | [Backend Cognito setup](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#backend-cognito-setup)                                                           |
| 21 | [Working Cruddur App - User signed in](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/week3.md#signed-in-user---working-cruddur-app-login)                                             |
                                                                                                                                       



## AWS Amplify install in env vars

![Configuring and Installing AWS amplify](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Install%20aws%20amplify.JPG)


## AWS Amplify import configuration     

![Importing AWS Amplify](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/aws%20amplify%20import.JPG)


## Updating Port startup (Public)

![Port startup configuration](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Update%20to%20gitpod%20yaml%20public%20ports.JPG)


## Updating the Backend AWS Cognito environment

![Cognito Backend fixes](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Cognito%20backend%20fixes.JPG)


## Configuring Login button behaviour

![Submit Button fix](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/editing%20on%20submit.JPG)


## Testing the Log in button behaviour for a response

![Log in invalid user test](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Incorrect%20username%20or%20password.JPG)


## Cognito - setup test-user via console
![Test User creation](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/test%20user.JPG)

## Cognito - review test-user configuration via console
![Sign in options](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/cognito%201.JPG)
![MFA](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/cognito%202.JPG)
![Required attributes](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/cognito%204.JPG)
![Configure message delivery](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/cognito%205.JPG)
![Userpool name](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/cognito%206.JPG)
![Advanced app client settings](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/cognito%207.JPG)


## Cognito - username and password sent to email
![Test User creation](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/cognito%20email%20password.JPG)

## Cognito - setting preferred username via console

![Preferred username config so as to work with the backend](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/setting%20preferred%20username.JPG)


## User confirmation email

![Confirm creation of user via email response](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/test%20user%20email%20setting%20temp%20password.JPG)


## Confirmed users account status changes to confirmed

![Users account status changes to confirmed after responding to email](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Status%20change%20pending%20to%20confirmed.JPG)

## Userpool creation

![Userpool creation](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/userpool%20creation.JPG)


## Cognito - user attributes

![User attributes](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/user%20attributes.JPG)


## Cognito User pool created

![Final User pool](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/userpool.JPG)


## Cognito - confirming email via terminal

![Force email confirmation in terminal](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/confirming%20email%20via%20terminal.JPG)

## Email status changed to confirmed

![Email status chnaged](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Userpool%20review.jpg)


## Cognito user pool dashboard

![User pool dashboard](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Cognito%20user%20pool.JPG)


## Cognito client ID

![Client ID](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Cognito%20client%20ID.JPG)


## Backend Cognito setup

![Cognito setup - backend env](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Backend%20cognito%20setup.JPG)


## Signed in user - Working Cruddur App Login

![User signed in](https://github.com/Stevecmd/aws-bootcamp-cruddur-2023/blob/main/journal/Week%203/Working%20app%20showing%20logged%20in%20user.JPG)
