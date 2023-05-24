# <img src="https://i.ibb.co/B3rpcB9/20220617-224257-0000-01.png"  width="30" height="30">  [Quick-Solution](https://quick-solution-2.web.app/)
## :page_facing_up: API Test Report
## :memo: How to run this project
### Run by Postman:
* Clone this repository.
* Import collection and environment file/link.
* Run the collection on Postman.
### Run by Newman:
* Clone this repository.
* Open cmd to the file location.
* Run Command:
-newman run Quick-Solution2.postman_collection.json -e Quick-Solution-Single-user.postman_environment.json
* Run Command for Report:
For html:
-newman run Quick-Solution2.postman_collection.json -e Quick-Solution-Single-user.postman_environment.json -r cli,html
For htmlextra:
newman run Quick-Solution2.postman_collection.json -e Quick-Solution-Single-user.postman_environment.json -r cli,htmlextra
### Technology used:
<img src="https://voyager.postman.com/logo/postman-logo-icon-orange.svg"  width="15" height="15"> Postman & Newman

### Prerequisite:
- Jdk
- Node Js
- Newman
- Html Report Library

### Newman and Report Installation Process:
- Newman Install Command:
npm install -g newman-reporter-htmlextra

- Newman Html Report Install Command:
npm install -g newman-reporter-htmlextra
