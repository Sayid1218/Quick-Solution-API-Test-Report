# <img src="https://i.ibb.co/B3rpcB9/20220617-224257-0000-01.png"  width="35" height="30">  [Quick-Solution](https://quick-solution-2.web.app/)
## :page_facing_up: API Test Report
## :memo: How to run this project
### 🖥 Run by Postman
* Clone this repository.
* Import collection and environment file/link.
* Run the collection on Postman.
### 🖥 Run by Newman
* Clone this repository.
* Open cmd to the file location.
* Run Command:
```console
newman run Quick-Solution2.postman_collection.json -e Quick-Solution-Single-user.postman_environment.json
```
* Run Command for Report:

For html:
```console
newman run Quick-Solution2.postman_collection.json -e Quick-Solution-Single-user.postman_environment.json -r cli,html
```
For htmlextra:
```console
newman run Quick-Solution2.postman_collection.json -e Quick-Solution-Single-user.postman_environment.json -r cli,htmlextra
```
### :technologist: Technology used
<img src="https://voyager.postman.com/logo/postman-logo-icon-orange.svg"  width="15" height="15"> Postman & Newman

### Prerequisite
- Jdk
- Node Js
- Newman
- Html Report Library

### Newman and Report Installation Process
- Newman Install Command:
``` console
npm install -g newman-reporter-htmlextra
```
- Newman Html Report Install Command:
``` console
npm install -g newman-reporter-htmlextra
```
### API Documentations
[PDF](https://drive.google.com/file/d/1cI9_7JVvtUjUSqY8ZTs3O4SYrdurudZS/view?usp=sharing)
#### Postman Documentations
[Postman](https://documenter.getpostman.com/view/24594715/2s93m4ZPT7)
## Test case list:
### Find Job By User
#### PUT
- Put user to Database and Collect accessToken.
- Put a applied job.
#### GET
- Find Job by Keyword.
- Get job Details.
- Get applied jobs.
#### DELETE
- Delete applied job.
### Post job by user
#### PUT
- Put user to database and collect accessToken.
#### POST
- Post a job.
#### GET
- Get posted job.
#### DELETE
- Delete posted job.
### Admin User
### GET
- Get all Jobs from database.
- Get an user information by email.
- Get all users from database.
- Get Category from database.
- Get Reviews.
- Get a email Admin or not.
### PUT
- Put category in database.
- Put a user to admin.
### POST
- Post a review.
### DELETE
- Delete user from database.
- Delete Review from database.

# Newman Report
![image](https://github.com/Sayid1218/Quick-Solution-API-Test-Report/assets/97175166/3b6cce36-6035-48f2-9f64-1dde7741dc13)
![image](https://github.com/Sayid1218/Quick-Solution-API-Test-Report/assets/97175166/c9d5fad0-ee9a-4ecc-8e67-4d1fa32a0c46)
![image](https://github.com/Sayid1218/Quick-Solution-API-Test-Report/assets/97175166/7890e125-7d8c-4c76-bc45-91221633f2de)

