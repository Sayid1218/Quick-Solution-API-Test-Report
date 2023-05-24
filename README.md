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
### Technology used
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
<body class="theme-dark">
<script>
    function setTheme(themeName) {
        localStorage.setItem('theme', themeName);
        document.body.className = themeName;
    }

    function toggleTheme() {
        if (localStorage.getItem('theme') === 'theme-light') {
            setTheme('theme-dark');
        } else {
            setTheme('theme-light');
        }
    }
</script>
  <div class="container">
        <div class="container">
            <label>Light</label>
            <label id="switch" class="switch">
                <input type="checkbox" onchange="toggleTheme()" id="slider">
                <span class="slider round"></span>
            </label>
            <label>Dark</label>
        </div>
        <div class="card">
        <div class="card-header">
            <ul class="nav nav-pills mb-3 nav-justified" id="pills-tab" role="tablist">
            <li class="nav-item bg-info active" data-toggle="tooltip" title="" data-original-title="Click to view the Summary">
                <a class="nav-link text-white" id="pills-summary-tab" data-toggle="pill" href="#pills-summary" role="tab" aria-controls="pills-summary" aria-selected="true">Summary</a>
            </li>
            <li class="nav-item bg-success" data-toggle="tooltip" title="" data-original-title="Click to view the Requests">
                <a class="nav-link text-white" id="pills-requests-tab" data-toggle="pill" href="#pills-requests" role="tab" aria-controls="pills-requests" aria-selected="false">Total Requests <span class="badge badge-light">21</span></a>
            </li>
            <li class="nav-item bg-danger" data-toggle="tooltip" title="" data-original-title="Click to view the Failed Tests">
                <a class="nav-link text-white" id="pills-failed-tab" data-toggle="pill" href="#pills-failed" role="tab" aria-controls="pills-failed" aria-selected="false">Failed Tests <span class="badge badge-light">0</span></a>
            </li>
            <li class="nav-item bg-warning" data-toggle="tooltip" title="" data-original-title="Click to view the Skipped Tests">
                <a class="nav-link text-white" id="pills-skipped-tab" data-toggle="pill" href="#pills-skipped" role="tab" aria-controls="pills-skipped" aria-selected="false">Skipped Tests <span class="badge badge-light">0</span></a>
            </li>
            </ul>
        <div class="tab-content" id="pills-tabContent">
            <div class="tab-pane fade show active" id="pills-summary" role="tabcard" aria-labelledby="pills-summary-tab">
<div class="row">
  <div class="col-md-9 col-lg-12 main">
   <h1 class="display-2 text-center">Newman Run Dashboard</h1>
   <h5 class="text-center">Wednesday, 24 May 2023 15:48:45</h5>
   <div class="row">
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-success">
      <div class="card-body bg-success">
       <div class="rotate">
        <i class="fa fa-retweet fa-5x"></i>
       </div>
       <h6 class="text-uppercase">Total Iterations</h6>
       <h1 class="display-1">1</h1>
      </div>
     </div>
    </div>
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-danger">
      <div class="card-body bg-success">
       <div class="rotate">
        <i class="fa fa-list fa-4x"></i>
       </div>
       <h6 class="text-uppercase">Total Assertions</h6>
       <h1 class="display-1">28</h1>
      </div>
     </div>
    </div>
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-info">
      <div class="card-body bg-success">
       <div class="rotate">
        <i class="fa fa-plus-circle fa-5x"></i>
       </div>
       <h6 class="text-uppercase">Total Failed Tests</h6>
       <h1 class="display-1">0</h1>
      </div>
     </div>
    </div>
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-warning">
      <div class="card-body bg-success">
       <div class="rotate">
        <i class="fa fa-share fa-5x"></i>
       </div>
       <h6 class="text-uppercase">Total Skipped Tests</h6>
       <h1 class="display-1">0</h1>
      </div>
     </div>
    </div>
   </div>
   <hr>
    <div class="row">
    <div class="col">
        <div class="row">
        <div class="col-sm-12 mb-3">
            <div class="card border-info">
                <div class="card-body">
                <h5 class="card-title text-uppercase text-white text-center bg-info">File Information</h5>
                <span><i class="fas fa-file-code"></i></span><strong> Collection:</strong> Quick-Solution2 Copy<br>
                
                <span><i class="fas fa-file-code"></i></span><strong> Environment:</strong> Quick-Solution-Single-user<br>
                </div>
            </div>
        </div>
        </div>
        <div class="row">
        <div class="col-sm-12 mb-3">
            <div class="card border-info">
                <div class="card-body">
                <h5 class="card-title text-uppercase text-white text-center bg-info">Timings and Data</h5>
                <span><i class="fas fa-stopwatch"></i></span><strong> Total run duration:</strong> 12s<br>
                <span><i class="fas fa-database"></i></span><strong> Total data received:</strong> 37.57KB<br>
                <span><i class="fas fa-stopwatch"></i></span><strong> Average response time:</strong> 490ms<br>
                </div>
            </div>
        </div>
        </div>
        <div class="row">
        <div class="col-sm-12 mb-3">
            <div class="table-responsive">
            <table class="table table-striped table-bordered">
                <thead class="thead-inverse">
                    <tr class="text-center">
                        <th class="text-uppercase">Summary Item</th>
                        <th class="text-uppercase">Total</th>
                        <th class="text-uppercase">Failed</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Requests</td>
                        <td class="text-center">21</td>
                        <td class="text-center">0</td>
                    </tr>
                    <tr>
                        <td>Prerequest Scripts</td>
                        <td class="text-center">1</td>
                        <td class="text-center">0</td>
                    </tr>
                    <tr>
                        <td>Test Scripts</td>
                        <td class="text-center">19</td>
                        <td class="text-center">0</td>
                    </tr>
                    <tr class="">
                        <td>Assertions</td>
                        <td class="text-center">28</td>
                        <td class="text-center">0</td>
                    </tr>
                    <tr class="">
                        <td>Skipped Tests</td>
                        <td class="text-center">0</td>
                        <td class="text-center">-</td>
                    </tr>
                </tbody>
            </table>
            </div>
        </div>
        </div>
    <hr>
   </div>
   </div>
  </div>
 </div>
        </div>
            <div class="tab-pane fade" id="pills-failed" role="tabcard" aria-labelledby="pills-failed-tab">
                <button id="topOfFailuresScreen" class="btn btn-outline-success btn-sm backToTop" onclick="topFunction()" style="display: none;">Go To Top</button>

                <div class="alert alert-success text-uppercase text-center">
                     <br><br><h1 class="text-center">There are no failed tests <span><i class="far fa-thumbs-up"></i></span></h1><br><br>
                </div>
            </div>

            <div class="tab-pane fade" id="pills-skipped" role="tabcard" aria-labelledby="pills-skipped-tab">
                <button id="topOfSkippedScreen" class="btn btn-outline-success btn-sm backToTop" onclick="topFunction()" style="display: none;">Go To Top</button>

                <div class="alert alert-success text-uppercase text-center">
                    <br><br><h1 class="text-center">There are no skipped tests <span><i class="far fa-thumbs-up"></i></span></h1><br><br>
                </div>
            </div>
            <div class="tab-pane fade" id="pills-requests" role="tabcard" aria-labelledby="pills-requests-tab">

            <button id="topOfRequestsScreen" class="btn btn-outline-success btn-sm backToTop" onclick="topFunction()" style="display: none;">Go To Top</button>

            <div class="btn-group float-right" role="group" aria-label="Button Group">
                <button id="openAll" class="btn btn-outline-success btn-sm float-right" style="text-align: center; width: 140px; display: block;">Expand Folders</button>
                <button id="openAllRequests" class="btn btn-outline-success btn-sm float-right" style="text-align: center; width: 140px; display: block;">Expand Requests</button>
            </div>

    <div class="text-uppercase" id="execution-menu">
        <h5>1 Iteration available to view</h5>
        
        <nav class="table-responsive">
        <ul class="nav single-line-tabs" id="iterationList">
        <li id="iteration-0" class="custom-tab itPassed" style="border-bottom: 3px solid rgb(3, 42, 51);">1</li></ul>
        </nav>
    </div>
    <h6 class="text-uppercase text-muted" id="iterationSelected" style="padding-top: 10px;">Iteration 1 selected</h6>
	<div class="tab-content" id="execution-data">
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-548b55f1-e86e-4d35-9836-d424a86c359f-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-548b55f1-e86e-4d35-9836-d424a86c359f-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Find Job by User / GET - 3 Requests in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-548b55f1-e86e-4d35-9836-d424a86c359f-iteration-0" class="collapse" aria-labelledby="folder-548b55f1-e86e-4d35-9836-d424a86c359f" style="border-bottom: none;">
            <div id="folder-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e" aria-expanded="false" aria-controls="collapse" id="requests-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e" class="collapsed text-white z-block">
                    Iteration: 1 - Find Job by Keyword <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e" class="collapse" aria-labelledby="requests-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/findjob?keyword=b" target="_blank">https://quick-solution.up.railway.app/findjob?keyword=b</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 1024ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 5.45KB</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">keyword</td>
                                                        <td class="text-wrap">{{keyword}}</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">1bcb4511-379f-4929-8844-f890986d306a</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">5576</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"15c8-Df7+Hd7gApsIKgMHeXhBmgh1tbI"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:33 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-27ed9ac9-aa8e-4c3e-9542-e65358da3ff6" class="prettyPrint hljs json">[
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b82e47ab528a7ef38d5a1c"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/vJKMsdx/php.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"NadiraCube"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"PHP Developer (paid internship)(Remote)"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"25,000"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur-1, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"We're looking for university students in their final year of studying Computer Science or recent Computer Science graduates. Applicants should be able to spend 25 hours per week working with our team to develop modern PHP web applications. The internship working hours will take place between 8 PM - 10 PM UTC+6, Monday through Friday with the remaining hours scheduled based on the candidate's availability."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"• Be a part of a talented and committed team\n• Solve interesting and challenging problems\n• Learn about proper software development and DevOps practices\n• Earn a lucrative allowance in an internship role"</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Having knowledge on following things is a plus:\n• PHP, Javascript, CSS and HTML.\n• PHP frameworks (Symfony, Laravel, etc) a plus\n• CMS (WordPress, Drupal) a plus\n• Basic knowledge of databases (MySQL)\n• Minimal conversational English skills"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"N/A"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01648854511"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"nadira15-12474@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-06"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-06"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b84365ab528a7ef38d5a1f"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/k0w5rhy/pngtree-cartoon-drawing-girl-download-image-1307074.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Shatabdi's Canvas"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Seller"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">" Online seller"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"4000"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Dhanmondi"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"We are searching for e online seller for our page"</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"\nExpert in online selling"</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"good communication"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Diploma"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"no"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01734280216"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"shatabdi15-12067@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-06"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-20"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"6463c90a4846d653b6b73075"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullah15-12377@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dcf8f67d09eadea169a73"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dd0b367d09eadea169a75"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dd1a067d09eadea169a77"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646ddb5a67d09eadea169a79"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  }
]</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-27ed9ac9-aa8e-4c3e-9542-e65358da3ff6">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_0_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_0_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_0"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_0" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_0" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_0" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_0" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_0" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Success</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-eeba57cd-d08a-4da5-bb40-2866f6d2a63c" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c" aria-expanded="false" aria-controls="collapse" id="requests-eeba57cd-d08a-4da5-bb40-2866f6d2a63c" class="collapsed text-white z-block">
                    Iteration: 1 - GET applied jobs <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c" class="collapse" aria-labelledby="requests-eeba57cd-d08a-4da5-bb40-2866f6d2a63c">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/myApplied/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/myApplied/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 403 - Forbidden</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 249ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 30B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar </td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">1b7d70ea-12a5-4332-8086-665fc2cec8e9</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">30</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"1e-NNRZhE06okBNKUTchJtjOZaGRqM"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:34 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-371926f4-fd7a-42e3-92b7-f3d0a0d9c236" class="prettyPrint hljs json">{
  <span class="hljs-attr">"massage"</span>: <span class="hljs-string">"Forbidden Access"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-371926f4-fd7a-42e3-92b7-f3d0a0d9c236">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_1_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_1_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_1"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_1" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_1" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_1" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_1" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_1" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Applied Jobs Gotted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-5f404d88-02a6-43fd-aaeb-ed09f694cff0" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0" aria-expanded="false" aria-controls="collapse" id="requests-5f404d88-02a6-43fd-aaeb-ed09f694cff0" class="collapsed text-white z-block">
                    Iteration: 1 - GET job details from DB <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0" class="collapse" aria-labelledby="requests-5f404d88-02a6-43fd-aaeb-ed09f694cff0">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/jobs/63b82e47ab528a7ef38d5a1c" target="_blank">https://quick-solution.up.railway.app/jobs/63b82e47ab528a7ef38d5a1c</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 463ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 1.36KB</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">dfa94c91-db75-49a8-b261-da17b854713b</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">1391</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"56f-rdkGPKXHbc/Ccdpt1+I9lsXSybI"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:34 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-cdee4140-6e45-4a76-98e3-4a51f8b4a06e" class="prettyPrint hljs json">{
  <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b82e47ab528a7ef38d5a1c"</span>,
  <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/vJKMsdx/php.jpg"</span>,
  <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"NadiraCube"</span>,
  <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
  <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"PHP Developer (paid internship)(Remote)"</span>,
  <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
  <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"25,000"</span>,
  <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur-1, Dhaka"</span>,
  <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"We're looking for university students in their final year of studying Computer Science or recent Computer Science graduates. Applicants should be able to spend 25 hours per week working with our team to develop modern PHP web applications. The internship working hours will take place between 8 PM - 10 PM UTC+6, Monday through Friday with the remaining hours scheduled based on the candidate's availability."</span>,
  <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"• Be a part of a talented and committed team\n• Solve interesting and challenging problems\n• Learn about proper software development and DevOps practices\n• Earn a lucrative allowance in an internship role"</span>,
  <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Having knowledge on following things is a plus:\n• PHP, Javascript, CSS and HTML.\n• PHP frameworks (Symfony, Laravel, etc) a plus\n• CMS (WordPress, Drupal) a plus\n• Basic knowledge of databases (MySQL)\n• Minimal conversational English skills"</span>,
  <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
  <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
  <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"N/A"</span>,
  <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01648854511"</span>,
  <span class="hljs-attr">"email"</span>: <span class="hljs-string">"nadira15-12474@diu.edu.bd"</span>,
  <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-06"</span>,
  <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-06"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-cdee4140-6e45-4a76-98e3-4a51f8b4a06e">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_2_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_2_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_2"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_2" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_2" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_2" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_2" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_2" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">JobDetails are gotted</td>
                                                    <td class="text-center bg-success">2</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">2</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-a4369510-7575-47d4-b620-11d381fa3689-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-a4369510-7575-47d4-b620-11d381fa3689-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Find Job by User / PUT - 2 Requests in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-a4369510-7575-47d4-b620-11d381fa3689-iteration-0" class="collapse" aria-labelledby="folder-a4369510-7575-47d4-b620-11d381fa3689" style="border-bottom: none;">
            <div id="folder-eddc7c2e-4a44-43a8-b6e3-233c57a21529" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529" aria-expanded="false" aria-controls="collapse" id="requests-eddc7c2e-4a44-43a8-b6e3-233c57a21529" class="collapsed text-white z-block">
                    Iteration: 1 - PUT a user to DB <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529" class="collapse" aria-labelledby="requests-eddc7c2e-4a44-43a8-b6e3-233c57a21529">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> PUT</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 475ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 299B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">b9c88f3c-e4f5-496b-a6fb-d1f9d374c35e</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">433</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-0" class="prettyPrint hljs json">{
  <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
  <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"{{Department}}"</span>,
  <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"{{Description}}"</span>,
  <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"{{Experience}}"</span>,
  <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"{{Phone}}"</span>,
  <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"{{Profile}}"</span>,
  <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"{{Student_ID}}"</span>,
  <span class="hljs-attr">"University"</span>: <span class="hljs-string">"{{University}}"</span>,
  <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"{{Year_OR_Semester}}"</span>,
  <span class="hljs-attr">"location"</span>: <span class="hljs-string">"{{location}}"</span>,
  <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"{{photoUrl}}"</span>,
  <span class="hljs-attr">"role"</span>: <span class="hljs-string">"{{role}}"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">299</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"12b-1uR1myudiJ8p4euK/S21oyOPG5Y"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:35 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-a7743890-51ea-425e-822d-4472a577fe08" class="prettyPrint hljs json">{
  <span class="hljs-attr">"result"</span>: {
    <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
    <span class="hljs-attr">"modifiedCount"</span>: <span class="hljs-number">1</span>,
    <span class="hljs-attr">"upsertedId"</span>: <span class="hljs-literal">null</span>,
    <span class="hljs-attr">"upsertedCount"</span>: <span class="hljs-number">0</span>,
    <span class="hljs-attr">"matchedCount"</span>: <span class="hljs-number">1</span>
  },
  <span class="hljs-attr">"accessToken"</span>: <span class="hljs-string">"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNSwiZXhwIjoxNjg0OTI1MzE1fQ.ZfhDnq4SNEdchNbnMEAfjWyfX6p9U97dHQSxfw621NU"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-a7743890-51ea-425e-822d-4472a577fe08">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_3_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_3_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_3"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_3" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_3" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_3" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_3" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_3" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Token Gotted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-75f7c382-c313-4d8a-9ad0-27f8231d725e" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e" aria-expanded="false" aria-controls="collapse" id="requests-75f7c382-c313-4d8a-9ad0-27f8231d725e" class="collapsed text-white z-block">
                    Iteration: 1 - Apply Job <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e" class="collapse" aria-labelledby="requests-75f7c382-c313-4d8a-9ad0-27f8231d725e">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> PUT</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/findjob/63b82e47ab528a7ef38d5a1c?email=abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/findjob/63b82e47ab528a7ef38d5a1c?email=abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 467ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 114B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">1ffaaf52-6078-48ae-8436-00f63d5f7a04</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">0</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">114</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"72-sPZIn6UAI6oF/BrhLkSjGF8KTD0"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:35 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-fb49c5fe-a037-4ea1-9e4f-a1f20aaeafed" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"modifiedCount"</span>: <span class="hljs-number">0</span>,
  <span class="hljs-attr">"upsertedId"</span>: <span class="hljs-string">"646ddd73ace09f222d3e2693"</span>,
  <span class="hljs-attr">"upsertedCount"</span>: <span class="hljs-number">1</span>,
  <span class="hljs-attr">"matchedCount"</span>: <span class="hljs-number">0</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-fb49c5fe-a037-4ea1-9e4f-a1f20aaeafed">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_4_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_4_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_4"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_4" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_4" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_4" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_4" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_4" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Applied</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Find Job by User / Delete - 1 Request in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81-iteration-0" class="collapse" aria-labelledby="folder-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81" style="border-bottom: none;">
            <div id="folder-73445db5-8e9d-4b11-b3f1-3314169e173b" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-73445db5-8e9d-4b11-b3f1-3314169e173b" aria-expanded="false" aria-controls="collapse" id="requests-73445db5-8e9d-4b11-b3f1-3314169e173b" class="collapsed text-white z-block">
                    Iteration: 1 - DELETE applied jobs <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-73445db5-8e9d-4b11-b3f1-3314169e173b" class="collapse" aria-labelledby="requests-73445db5-8e9d-4b11-b3f1-3314169e173b">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> DELETE</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/myApplied/63b82e47ab528a7ef38d5a1c" target="_blank">https://quick-solution.up.railway.app/myApplied/63b82e47ab528a7ef38d5a1c</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 464ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 38B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNSwiZXhwIjoxNjg0OTI1MzE1fQ.ZfhDnq4SNEdchNbnMEAfjWyfX6p9U97dHQSxfw621NU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">6389508f-9eee-4235-8da1-5278fba208ed</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">38</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"26-fgR5yLHQ1Hpp6zDESHaY9wJreYE"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-516c8e8a-1d1f-4d01-9329-b344ca8751a8" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"deletedCount"</span>: <span class="hljs-number">1</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-516c8e8a-1d1f-4d01-9329-b344ca8751a8">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_5_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_5_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_5"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_5" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_5" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_5" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_5" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_5" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Deleted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-cd20c794-0e9f-4762-8ce4-997b4cc85feb-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-cd20c794-0e9f-4762-8ce4-997b4cc85feb-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Post Job by User / PUT - 1 Request in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-cd20c794-0e9f-4762-8ce4-997b4cc85feb-iteration-0" class="collapse" aria-labelledby="folder-cd20c794-0e9f-4762-8ce4-997b4cc85feb" style="border-bottom: none;">
            <div id="folder-07bf8973-f568-4e38-8cff-9634f5a27ac3" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3" aria-expanded="false" aria-controls="collapse" id="requests-07bf8973-f568-4e38-8cff-9634f5a27ac3" class="collapsed text-white z-block">
                    Iteration: 1 - PUT a user to DB Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3" class="collapse" aria-labelledby="requests-07bf8973-f568-4e38-8cff-9634f5a27ac3">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> PUT</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 469ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 299B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">1d03287a-ae5d-4fe1-8c42-b1b1f4bfadc0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">1889</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-0" class="prettyPrint hljs json">{
  <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
  <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
  <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I am a web developer who creates websites and applications. I develop websites that are user friendly, attractive and highly functional. I use the latest technologies and coding languages, such as HTML, CSS, JavaScript, and PHP, to create websites that are compatible with all browsers and platforms. I also use frameworks such as WordPress and Bootstrap to create websites quickly and efficiently. In addition, I also develop backend applications to help manage databases and complete complex tasks"</span>,
  <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"web developer is responsible for creating and maintaining websites. They design, code, and build websites, using a variety of web programming languages and technologies. Web developers must also have an understanding of usability and accessibility, as well as an understanding of web standards and best practices.\n\nTo become a successful web developer, individuals must have strong technical skills, an eye for detail, and a good working knowledge of web technologies and development tools. They must also possess strong problem-solving and communication skills, as well as the ability to work independently and collaboratively.\n\nTo stay up-to-date on the latest web development trends and technologies, web developers usually attend conferences, read industry publications, and participate in online forums. Additionally, web developers may also need to be familiar with content management systems (CMS) in order to manage the content on websites."</span>,
  <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
  <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
  <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
  <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversit}"</span>,
  <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
  <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Dhaka"</span>,
  <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/WcDh5yY/20201216061303-IMG-0156-clipdrop-relight.jpg"</span>,
  <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">299</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"12b-jSeeNLhe83vopC7ISPpaWi6o8MU"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-cafa0548-4f00-46a0-a2b8-2d7a102ac55d" class="prettyPrint hljs json">{
  <span class="hljs-attr">"result"</span>: {
    <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
    <span class="hljs-attr">"modifiedCount"</span>: <span class="hljs-number">1</span>,
    <span class="hljs-attr">"upsertedId"</span>: <span class="hljs-literal">null</span>,
    <span class="hljs-attr">"upsertedCount"</span>: <span class="hljs-number">0</span>,
    <span class="hljs-attr">"matchedCount"</span>: <span class="hljs-number">1</span>
  },
  <span class="hljs-attr">"accessToken"</span>: <span class="hljs-string">"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-cafa0548-4f00-46a0-a2b8-2d7a102ac55d">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_6_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_6_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_6"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_6" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_6" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_6" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_6" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_6" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Token Gotted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-9e323c4a-8667-4374-a10b-2995c7c84562-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-9e323c4a-8667-4374-a10b-2995c7c84562-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Post Job by User / POST - 1 Request in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-9e323c4a-8667-4374-a10b-2995c7c84562-iteration-0" class="collapse" aria-labelledby="folder-9e323c4a-8667-4374-a10b-2995c7c84562" style="border-bottom: none;">
            <div id="folder-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9" aria-expanded="false" aria-controls="collapse" id="requests-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9" class="collapsed text-white z-block">
                    Iteration: 1 - POST a Job Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9" class="collapse" aria-labelledby="requests-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/jobs" target="_blank">https://quick-solution.up.railway.app/jobs</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 468ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 61B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">1178cd45-8d4b-491f-8052-72aff019baab</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">869</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-0" class="prettyPrint hljs json">{
  <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
  <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
  <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
  <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
  <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
  <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
  <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
  <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
  <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
  <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
  <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
  <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
  <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
  <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
  <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
  <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
  <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">61</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"3d-7xBEx+ZHPY9SjWw+aM5XTk6Oudc"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-7212767a-a3cb-45b0-b4d6-1e37e30313e4" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"insertedId"</span>: <span class="hljs-string">"646ddd7567d09eadea169a7c"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-7212767a-a3cb-45b0-b4d6-1e37e30313e4">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_7_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_7_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_7"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_7" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_7" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_7" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_7" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_7" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Job Posted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-6c9a5aa5-57d3-41d7-8de2-9057de500785-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-6c9a5aa5-57d3-41d7-8de2-9057de500785-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Post Job by User / GET - 1 Request in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-6c9a5aa5-57d3-41d7-8de2-9057de500785-iteration-0" class="collapse" aria-labelledby="folder-6c9a5aa5-57d3-41d7-8de2-9057de500785" style="border-bottom: none;">
            <div id="folder-3a7ced69-9d5c-42bb-a382-962812c5ade3" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3" aria-expanded="false" aria-controls="collapse" id="requests-3a7ced69-9d5c-42bb-a382-962812c5ade3" class="collapsed text-white z-block">
                    Iteration: 1 - GET posted jobs from DB Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3" class="collapse" aria-labelledby="requests-3a7ced69-9d5c-42bb-a382-962812c5ade3">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/myjobs/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/myjobs/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 463ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 3.48KB</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">813f548c-5504-4210-8c6a-9eee68ba33b0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">3561</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"de9-NpMDG1sCwG9CgCRBql/sKlV84og"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:38 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-28d65915-192b-4763-8445-7fd19dfc796c" class="prettyPrint hljs json">[
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dcf8f67d09eadea169a73"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dd0b367d09eadea169a75"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dd1a067d09eadea169a77"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646ddb5a67d09eadea169a79"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646ddd7567d09eadea169a7c"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  }
]</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-28d65915-192b-4763-8445-7fd19dfc796c">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_8_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_8_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_8"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_8" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_8" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_8" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_8" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_8" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">JobDetails</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-0e2a6797-c9e5-43ae-90aa-1f0c1c907830-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-0e2a6797-c9e5-43ae-90aa-1f0c1c907830-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Post Job by User / DELETE - 1 Request in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-0e2a6797-c9e5-43ae-90aa-1f0c1c907830-iteration-0" class="collapse" aria-labelledby="folder-0e2a6797-c9e5-43ae-90aa-1f0c1c907830" style="border-bottom: none;">
            <div id="folder-6c86f601-cf57-41ee-9144-beeeb611895c" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-6c86f601-cf57-41ee-9144-beeeb611895c" aria-expanded="false" aria-controls="collapse" id="requests-6c86f601-cf57-41ee-9144-beeeb611895c" class="collapsed text-white z-block">
                    Iteration: 1 - Delete Job by Jobid Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-6c86f601-cf57-41ee-9144-beeeb611895c" class="collapse" aria-labelledby="requests-6c86f601-cf57-41ee-9144-beeeb611895c">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> DELETE</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/deletejob/646ddd7567d09eadea169a7c" target="_blank">https://quick-solution.up.railway.app/deletejob/646ddd7567d09eadea169a7c</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 467ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 38B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">b3cff638-e6a0-4b7a-8d97-fd5bd83b9144</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">38</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"26-fgR5yLHQ1Hpp6zDESHaY9wJreYE"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:38 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-83cd7526-a490-40ff-bdae-5f2e1407a924" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"deletedCount"</span>: <span class="hljs-number">1</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-83cd7526-a490-40ff-bdae-5f2e1407a924">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_9_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_9_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_9"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_9" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_9" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_9" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_9" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_9" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Deleted Job</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-38b8045e-22e4-4ae7-b42a-ba9399265103-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-38b8045e-22e4-4ae7-b42a-ba9399265103-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Admin users / GET - 6 Requests in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-38b8045e-22e4-4ae7-b42a-ba9399265103-iteration-0" class="collapse" aria-labelledby="folder-38b8045e-22e4-4ae7-b42a-ba9399265103" style="border-bottom: none;">
            <div id="folder-eced55c6-6fc9-413c-91b7-c0a3e40d190e" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e" aria-expanded="false" aria-controls="collapse" id="requests-eced55c6-6fc9-413c-91b7-c0a3e40d190e" class="collapsed text-white z-block">
                    Iteration: 1 - GET All Jobs from DB <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e" class="collapse" aria-labelledby="requests-eced55c6-6fc9-413c-91b7-c0a3e40d190e">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/jobs" target="_blank">https://quick-solution.up.railway.app/jobs</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 461ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 7.9KB</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">50cea205-6ffc-46bc-81ca-5dc8082e220e</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">8088</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"1f98-6uGjRUQQqtIeS54kyHGgZBzaGEE"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:39 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-0232b4be-3d10-4cc1-a8de-ca5f2477651a" class="prettyPrint hljs json">[
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b8260dab528a7ef38d5a1a"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/9p2XtpK/fitted.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Nadira Rider"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Delivery"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Food Delivery"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"10,000-14,000"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur-1, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"If you want  to find Delivery Rider jobs easily online, then visit Nadira Rider and choose from your jobs."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"A rider's job is to maintain a specific route or area to collect or deliver packages. You often used bicycles or motorcycles to perform their duties. Their duties and responsibilities include writing logs and reports, collecting payment for deliveries, and informing customers of new products and services."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"1.Proven experience as a Driver.\n2.A valid driver's license.\n3.A clean driving record.\n4.Minimum visual acuity of 20/50 (or corrected to 20/50)\n5.Familiarity with GPS devices.\n6.Knowledge of area roads and 7.neighborhoods.\n8.Ability to lift heavy packages and luggage."</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Diploma"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"N/A"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01648854511"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"nadira15-12474@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-06"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-06"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b82911ab528a7ef38d5a1b"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/jzRGX5F/download.png"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Nadira Anjum"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Tutions"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"English O level Home tutor"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"5000"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur-1, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"English O level home tutor"</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"Time maintain, Good behavior etc "</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"expert and professional in English language."</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"N/A"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01648854511"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"nadira15-12474@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-06"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-06"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b82e47ab528a7ef38d5a1c"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/vJKMsdx/php.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"NadiraCube"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"PHP Developer (paid internship)(Remote)"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"25,000"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur-1, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"We're looking for university students in their final year of studying Computer Science or recent Computer Science graduates. Applicants should be able to spend 25 hours per week working with our team to develop modern PHP web applications. The internship working hours will take place between 8 PM - 10 PM UTC+6, Monday through Friday with the remaining hours scheduled based on the candidate's availability."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"• Be a part of a talented and committed team\n• Solve interesting and challenging problems\n• Learn about proper software development and DevOps practices\n• Earn a lucrative allowance in an internship role"</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Having knowledge on following things is a plus:\n• PHP, Javascript, CSS and HTML.\n• PHP frameworks (Symfony, Laravel, etc) a plus\n• CMS (WordPress, Drupal) a plus\n• Basic knowledge of databases (MySQL)\n• Minimal conversational English skills"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"N/A"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01648854511"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"nadira15-12474@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-06"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-06"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b84365ab528a7ef38d5a1f"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/k0w5rhy/pngtree-cartoon-drawing-girl-download-image-1307074.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Shatabdi's Canvas"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Seller"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">" Online seller"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"4000"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Dhanmondi"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"We are searching for e online seller for our page"</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"\nExpert in online selling"</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"good communication"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Diploma"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"no"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01734280216"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"shatabdi15-12067@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-06"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-20"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63d3909cced5f0e50b945532"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/b72gzdH/logo.png"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Sayid IT"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Other"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Customer Service"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"Part-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Negotiable"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I need customer service  assistant. I have shop near Mirpur 1. I need a student who can manage my customer smartly."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"Manage Customer Smartly. Handle situation smartly."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Smart, Good looking, Well behaver and have good time management."</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"As par work."</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01927777399"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullah15-12377@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-01-31"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"6463c90a4846d653b6b73075"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullah15-12377@diu.edu.bd"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dcf8f67d09eadea169a73"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dd0b367d09eadea169a75"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dd1a067d09eadea169a77"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646ddb5a67d09eadea169a79"</span>,
    <span class="hljs-attr">"LogoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/JpBy401/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"AuthorName"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Category"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"Post"</span>: <span class="hljs-string">"Fix Windows Software issue"</span>,
    <span class="hljs-attr">"Type"</span>: <span class="hljs-string">"One-time"</span>,
    <span class="hljs-attr">"Salary"</span>: <span class="hljs-string">"Depemds on work"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I ahve computer and it has some issues. You have to check all ."</span>,
    <span class="hljs-attr">"Responsibilities"</span>: <span class="hljs-string">"If you are a it student it will be better. Have knowledge about PC."</span>,
    <span class="hljs-attr">"Reqiuronment"</span>: <span class="hljs-string">"Time needed minimum 3 hour"</span>,
    <span class="hljs-attr">"Vacancy"</span>: <span class="hljs-string">"1"</span>,
    <span class="hljs-attr">"Educational_Requirements"</span>: <span class="hljs-string">"Batchelor"</span>,
    <span class="hljs-attr">"Compensation_Other_Benefits"</span>: <span class="hljs-string">"n/a"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Published_On"</span>: <span class="hljs-string">"2023-01-27"</span>,
    <span class="hljs-attr">"Application_Deadline"</span>: <span class="hljs-string">"2023-02-10"</span>
  }
]</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-0232b4be-3d10-4cc1-a8de-ca5f2477651a">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_10_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_10_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_10"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_10" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_10" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_10" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_10" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_10" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Jobs are gotted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-b719159f-acfa-479c-9e12-c118ad814145" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-b719159f-acfa-479c-9e12-c118ad814145" aria-expanded="false" aria-controls="collapse" id="requests-b719159f-acfa-479c-9e12-c118ad814145" class="collapsed text-white z-block">
                    Iteration: 1 - GET an user information by email <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-b719159f-acfa-479c-9e12-c118ad814145" class="collapse" aria-labelledby="requests-b719159f-acfa-479c-9e12-c118ad814145">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 460ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 1.79KB</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">376c71fc-7934-4188-a1e2-f9d96658ca07</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">1836</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"72c-zjLW+6WufWBssExAuy5XKdj5I/g"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:39 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-772c248b-3505-42c1-b40a-d1fe6e75ee45" class="prettyPrint hljs json">{
  <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646b44a5ace09f222d24d1e8"</span>,
  <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
  <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
  <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I am a web developer who creates websites and applications. I develop websites that are user friendly, attractive and highly functional. I use the latest technologies and coding languages, such as HTML, CSS, JavaScript, and PHP, to create websites that are compatible with all browsers and platforms. I also use frameworks such as WordPress and Bootstrap to create websites quickly and efficiently. In addition, I also develop backend applications to help manage databases and complete complex tasks"</span>,
  <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"web developer is responsible for creating and maintaining websites. They design, code, and build websites, using a variety of web programming languages and technologies. Web developers must also have an understanding of usability and accessibility, as well as an understanding of web standards and best practices.\n\nTo become a successful web developer, individuals must have strong technical skills, an eye for detail, and a good working knowledge of web technologies and development tools. They must also possess strong problem-solving and communication skills, as well as the ability to work independently and collaboratively.\n\nTo stay up-to-date on the latest web development trends and technologies, web developers usually attend conferences, read industry publications, and participate in online forums. Additionally, web developers may also need to be familiar with content management systems (CMS) in order to manage the content on websites."</span>,
  <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
  <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
  <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
  <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversit}"</span>,
  <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
  <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Dhaka"</span>,
  <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/WcDh5yY/20201216061303-IMG-0156-clipdrop-relight.jpg"</span>,
  <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-772c248b-3505-42c1-b40a-d1fe6e75ee45">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_11_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_11_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_11"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_11" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_11" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_11" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_11" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_11" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">User Verified</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-fb0e55a3-06db-4273-b951-db7c486363db" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-fb0e55a3-06db-4273-b951-db7c486363db" aria-expanded="false" aria-controls="collapse" id="requests-fb0e55a3-06db-4273-b951-db7c486363db" class="collapsed text-white z-block">
                    Iteration: 1 - GET All users from DB <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-fb0e55a3-06db-4273-b951-db7c486363db" class="collapse" aria-labelledby="requests-fb0e55a3-06db-4273-b951-db7c486363db">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/users" target="_blank">https://quick-solution.up.railway.app/users</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 694ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 13.05KB</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">97e8ba0f-b3c0-4fe4-b6e6-c985c936aae5</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">13368</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"3438-GXIeEVtOs38nilGSemzecvUq9GU"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:40 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-3b0a9cc0-990f-4258-8478-5e501e6296dc" class="prettyPrint hljs json">[
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63935426f32253e295f888aa"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"rafsun4566@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"An app developer is a software engineer or programmer who creates applications (apps) for mobile devices such as smartphones and tablets. They develop apps for iOS and Android operating systems, as well as other mobile platforms. App developers are responsible for the entire software development process and must be proficient in coding, problem solving, software architecture, and design. They must also have experience with the latest technologies and platforms in order to create the most efficient and user-friendly apps. App developers must have a strong understanding of user interface design and be able to create intuitive and engaging user experiences."</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"App development, MS word, Adobe XD, Java etc."</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Rafsun Eshrar"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"124786565656"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12376"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/8jspqy2/243007154-3044692155777654-2172741054242877438-n.jpg"</span>,
    <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63960943d2f4496b9d72742f"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"nadira12@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"A CSE student is someone who is enrolled in a computer science and engineering program. They are typically interested in the cutting edge of technology, and may have an aptitude for mathematics and problem-solving. CSE students often gain a broad range of technical skills, including knowledge of computational theory, programming languages, operating systems, and computer hardware. They may also learn to design and implement complex software systems. CSE students typically pursue careers in fields related to computer science, such as software engineering, information technology, data science, and web development."</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"As a CSE student, you can expect to gain a wide range of technical, problem-solving, and communication skills. You will be exposed to a variety of programming languages, software development tools, and operating systems. You will learn how to design, code, and debug computer programs, as well as how to develop databases. You will also learn how to write and design technical documents, troubleshoot hardware and software problems, and work in teams. In addition, you will be exposed to the principles of computer science, including algorithms, data structures, and artificial intelligence."</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Rafa"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01576646457"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12402"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/g4QQ49n/image1.jpg"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63960b63d2f4496b9d754adc"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"ride12@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"A CSE student is a person who has chosen to pursue a degree in the field of computer science and engineering. They are typically highly motivated, analytical, and detail-oriented individuals who are passionate about technology and problem-solving. CSE students are often well-versed in a variety of programming languages, software engineering principles, and computer architecture. They are also knowledgeable in mathematics, physics, and other scientific disciplines that are associated with computer science. CSE students enjoy the challenge of tackling complex problems and developing innovative solutions. They have an insatiable curiosity and an eagerness to stay up to date on the latest technological advancements. After completing a CSE degree, many students find rewarding careers in software engineering, artificial intelligence, cybersecurity, and other related fields."</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"As a CSE student, you can expect to gain a wide range of technical, problem-solving, and communication skills. You will be exposed to a variety of programming languages, software development tools, and operating systems. You will learn how to design, code, and debug computer programs, as well as how to develop databases. You will also learn how to write and design technical documents, troubleshoot hardware and software problems, and work in teams. In addition, you will be exposed to the principles of computer science, including algorithms, data structures, and artificial intelligence."</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Rhride"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"015735757878"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12358"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Gulshan, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/Jpkn9Pt/318620870-3373916832889879-9175171191859186222-n.jpg"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63aea1a5e4f82e27e0bb4d74"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"sayid1234@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"jaijfajfdjfk"</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"zkvkljjkdjvkjk"</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Abdullah Sayid"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01763398915"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/zbV1FLc/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63aea577e4f82e27e0c08216"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"kingsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"vhghghgh"</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"hhghgg"</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"kings Photography"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"878786877564"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/zbV1FLc/photo-2022-11-29-08-45-36.jpg"</span>,
    <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63aea786e4f82e27e0c3476e"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I am searching tuitions"</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"Tuition, Project"</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"12352525225"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b2a2927d78a74efcf59b4b"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"gamal12@gmail.com"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b2a3757d78a74efcf714f2"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"ei12@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"3egr"</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"dgfssssss"</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"King"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"54312"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/9VzmBMB/318933858-668059964719703-5983351848532693540-n.jpg"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b81c1eec791d4a07109999"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"shatabdi15-12067@diu.edu.bd"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"cse"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">" am a student"</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"no"</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Shatabdi Roy 191-15-12067"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01734280216"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International University"</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"2019-2024"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Dhanmondi"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/wyYMfhH/321602420-1200961513872298-4832220098775612229-n.jpg"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b81d30ec791d4a071290fd"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"nadira15-12474@diu.edu.bd"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"Computer Science and Engineering"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"My name is Nadira Anjum. I'm  a student at Daffodil International University, Dept of CSE."</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"Some core computer science courses you may cover include theory of computation, fundamentals of computer science, compliers and operating systems, information theory, basic programming, systems and architecture, software development and testing, web applications and databases, algorithms and data structures, and .so on."</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Nadira Anjum"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01648854511"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12474"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International University"</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"final year, Defense on going"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mirpur-1, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/vxZYhhZ/323454936-928644308507637-8155777678787713781-n-1.jpg"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b93f02ec791d4a07b50e4b"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"ei1234567@gmail.com"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63d39cf20b43d3e3f910e430"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"atik15-12802@diu.edu.bd"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63e23df600d193dde0bbc22f"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"shahriare.akash@gmail.com"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"6468f583ace09f222d53402f"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullah1218@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I am a web developer who creates websites and applications. I develop websites that are user friendly, attractive and highly functional. I use the latest technologies and coding languages, such as HTML, CSS, JavaScript, and PHP, to create websites that are compatible with all browsers and platforms. I also use frameworks such as WordPress and Bootstrap to create websites quickly and efficiently. In addition, I also develop backend applications to help manage databases and complete complex tasks."</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"web developer is responsible for creating and maintaining websites. They design, code, and build websites, using a variety of web programming languages and technologies. Web developers must also have an understanding of usability and accessibility, as well as an understanding of web standards and best practices.\n\nTo become a successful web developer, individuals must have strong technical skills, an eye for detail, and a good working knowledge of web technologies and development tools. They must also possess strong problem-solving and communication skills, as well as the ability to work independently and collaboratively.\n\nTo stay up-to-date on the latest web development trends and technologies, web developers usually attend conferences, read industry publications, and participate in online forums. Additionally, web developers may also need to be familiar with content management systems (CMS) in order to manage the content on websites."</span>,
    <span class="hljs-attr">"Name"</span>: <span class="hljs-string">"Abdullah Mohammod Sayid Boiah"</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity "</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/WcDh5yY/20201216061303-IMG-0156-clipdrop-relight.jpg"</span>,
    <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646b44a5ace09f222d24d1e8"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullahsayid1218@gmail.com"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I am a web developer who creates websites and applications. I develop websites that are user friendly, attractive and highly functional. I use the latest technologies and coding languages, such as HTML, CSS, JavaScript, and PHP, to create websites that are compatible with all browsers and platforms. I also use frameworks such as WordPress and Bootstrap to create websites quickly and efficiently. In addition, I also develop backend applications to help manage databases and complete complex tasks"</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"web developer is responsible for creating and maintaining websites. They design, code, and build websites, using a variety of web programming languages and technologies. Web developers must also have an understanding of usability and accessibility, as well as an understanding of web standards and best practices.\n\nTo become a successful web developer, individuals must have strong technical skills, an eye for detail, and a good working knowledge of web technologies and development tools. They must also possess strong problem-solving and communication skills, as well as the ability to work independently and collaboratively.\n\nTo stay up-to-date on the latest web development trends and technologies, web developers usually attend conferences, read industry publications, and participate in online forums. Additionally, web developers may also need to be familiar with content management systems (CMS) in order to manage the content on websites."</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"01580394350"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversit}"</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/WcDh5yY/20201216061303-IMG-0156-clipdrop-relight.jpg"</span>,
    <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646b5d2face09f222d3bd2a5"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullah15-12377@diu.edu.bd"</span>,
    <span class="hljs-attr">"Department"</span>: <span class="hljs-string">"CSE"</span>,
    <span class="hljs-attr">"Description"</span>: <span class="hljs-string">"I am a web developer who creates websites and applications. I develop websites that are user friendly, attractive and highly functional. I use the latest technologies and coding languages, such as HTML, CSS, JavaScript, and PHP, to create websites that are compatible with all browsers and platforms. I also use frameworks such as WordPress and Bootstrap to create websites quickly and efficiently. In addition, I also develop backend applications to help manage databases and complete complex tasks."</span>,
    <span class="hljs-attr">"Experience"</span>: <span class="hljs-string">"web developer is responsible for creating and maintaining websites. They design, code, and build websites, using a variety of web programming languages and technologies. Web developers must also have an understanding of usability and accessibility, as well as an understanding of web standards and best practices.\n\nTo become a successful web developer, individuals must have strong technical skills, an eye for detail, and a good working knowledge of web technologies and development tools. They must also possess strong problem-solving and communication skills, as well as the ability to work independently and collaboratively.\n\nTo stay up-to-date on the latest web development trends and technologies, web developers usually attend conferences, read industry publications, and participate in online forums. Additionally, web developers may also need to be familiar with content management systems (CMS) in order to manage the content on websites."</span>,
    <span class="hljs-attr">"Phone"</span>: <span class="hljs-string">"1580394350"</span>,
    <span class="hljs-attr">"Profile"</span>: <span class="hljs-string">"Updated"</span>,
    <span class="hljs-attr">"Student_ID"</span>: <span class="hljs-string">"191-15-12377"</span>,
    <span class="hljs-attr">"University"</span>: <span class="hljs-string">"Daffodil International Unversity"</span>,
    <span class="hljs-attr">"Year_OR_Semester"</span>: <span class="hljs-string">"4rth"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"photoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/WcDh5yY/20201216061303-IMG-0156-clipdrop-relight.jpg"</span>,
    <span class="hljs-attr">"role"</span>: <span class="hljs-string">"admin"</span>
  }
]</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-3b0a9cc0-990f-4258-8478-5e501e6296dc">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_12_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_12_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_12"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_12" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_12" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_12" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_12" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_12" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Body matches string</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-52b76027-7808-47a8-923b-29d76b54131f" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-52b76027-7808-47a8-923b-29d76b54131f" aria-expanded="false" aria-controls="collapse" id="requests-52b76027-7808-47a8-923b-29d76b54131f" class="collapsed text-white z-block">
                    Iteration: 1 - GET category from DB <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-52b76027-7808-47a8-923b-29d76b54131f" class="collapse" aria-labelledby="requests-52b76027-7808-47a8-923b-29d76b54131f">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/categories" target="_blank">https://quick-solution.up.railway.app/categories</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 458ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 933B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">1102e1f2-581b-47a6-b7f8-36005ad05f60</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">933</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"3a5-9PXyp4TMDxrswg0vOlnc15jPZJA"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:41 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-e49e8710-558a-4192-8a09-e0f36cfa74ee" class="prettyPrint hljs json">[
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b0a85ff9c7bd62c21b052"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Software Fix"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/zHjrRP3/Software.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b0e95ff9c7bd62c26ae66"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Project"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/DLfpTQt/Project.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b105cff9c7bd62c28e53e"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Photography"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/k0gBVJk/Photography.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b1132ff9c7bd62c29edc5"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Call Center"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/z7pkmKd/phone.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b114fff9c7bd62c2a128e"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"It Assistant"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/4fG7v5w/Assistent.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b11beff9c7bd62c2a9a3a"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Seller"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/B4yNbZq/Seller.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b1b46ff9c7bd62c36669e"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Delivery"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/pRDs4q9/Delevery.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b6d73829b16fac7f1fd33"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Volunteer"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/hFgGmBB/Volunteer.png"</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"638b734a829b16fac7f95853"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Other"</span>,
    <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/2cHLR6M/Other.png"</span>
  }
]</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-e49e8710-558a-4192-8a09-e0f36cfa74ee">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_13_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_13_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_13"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_13" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_13" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_13" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_13" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_13" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                                
                                                
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">_id here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="even">
                                                    <td class="sorting_1">Category gotted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="odd">
                                                    <td class="sorting_1">Logo here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="even">
                                                    <td class="sorting_1">Name here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">4</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-8b8ac03a-f031-4422-850f-10c74b16f072" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-8b8ac03a-f031-4422-850f-10c74b16f072" aria-expanded="false" aria-controls="collapse" id="requests-8b8ac03a-f031-4422-850f-10c74b16f072" class="collapsed text-white z-block">
                    Iteration: 1 - GET Reviews <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-8b8ac03a-f031-4422-850f-10c74b16f072" class="collapse" aria-labelledby="requests-8b8ac03a-f031-4422-850f-10c74b16f072">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/reviews" target="_blank">https://quick-solution.up.railway.app/reviews</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 460ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 2.45KB</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">e1a38fe1-1728-4dc0-b3c4-c877afef02de</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">2511</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"9cf-fwQfGSGAmmrJG/X+dpi4oxe1z+M"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:41 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-c8f157e5-aecb-48fd-befb-42214f128b0a" class="prettyPrint hljs json">[
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"6394b724da0d115ad9d21dc7"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Abdullah Sayid"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/WcDh5yY/20201216061303-IMG-0156-clipdrop-relight.jpg"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"abdullah15-12377@diu.edu.bd"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Gulshan, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"It is wander full website. To find out jobs, part-time projects, temporary works. Students can find their suitable jobs and do it their own working time."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"63b1a80aab528a7ef38d5a18"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646476ce4846d653b6b73076"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Rafa"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/vxZYhhZ/323454936-928644308507637-8155777678787713781-n-1.jpg"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Bangladesh"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"Overall Mch becomes your work family. I feel the love man. Really though if you have a drive to help people and be appreciated for it Mch is for you."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dc25d67d09eadea169a6c"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dcc9267d09eadea169a6d"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dccb267d09eadea169a6e"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dce6e67d09eadea169a70"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dcebb67d09eadea169a71"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
  },
  {
    <span class="hljs-attr">"_id"</span>: <span class="hljs-string">"646dcee067d09eadea169a72"</span>,
    <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
    <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
    <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
    <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
    <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
  }
]</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-c8f157e5-aecb-48fd-befb-42214f128b0a">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_14_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_14_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_14"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_14" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_14" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_14" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_14" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_14" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                                
                                                
                                                
                                                
                                                
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">_id here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="even">
                                                    <td class="sorting_1">Email here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="odd">
                                                    <td class="sorting_1">Image here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="even">
                                                    <td class="sorting_1">Location here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="odd">
                                                    <td class="sorting_1">Name here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="even">
                                                    <td class="sorting_1">Reviews gotted</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr><tr role="row" class="odd">
                                                    <td class="sorting_1">Reviewtext here</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">7</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-81093223-ad2e-45ab-9d70-655caa29d027" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-81093223-ad2e-45ab-9d70-655caa29d027" aria-expanded="false" aria-controls="collapse" id="requests-81093223-ad2e-45ab-9d70-655caa29d027" class="collapsed text-white z-block">
                    Iteration: 1 - GET a email Admin or not <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-81093223-ad2e-45ab-9d70-655caa29d027" class="collapse" aria-labelledby="requests-81093223-ad2e-45ab-9d70-655caa29d027">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/user/admin/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/user/admin/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 459ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 14B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">b11bb723-2762-4291-8dc8-45ba7e25fca8</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">14</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"e-x0QxBxSD57ubamUKWdrrFz36k7o"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:42 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-95e94ac8-0587-4bac-bbbe-b9a138a45724" class="prettyPrint hljs json">{
  <span class="hljs-attr">"admin"</span>: <span class="hljs-literal">true</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-95e94ac8-0587-4bac-bbbe-b9a138a45724">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_15_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_15_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_15"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_15" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_15" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_15" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_15" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_15" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">abdullahsayid1218@gmail.com is an admin</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-e807cb85-0182-4073-9d05-a43a0e9cf410-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-e807cb85-0182-4073-9d05-a43a0e9cf410-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Admin users / PUT - 2 Requests in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-e807cb85-0182-4073-9d05-a43a0e9cf410-iteration-0" class="collapse" aria-labelledby="folder-e807cb85-0182-4073-9d05-a43a0e9cf410" style="border-bottom: none;">
            <div id="folder-eb212d7c-2281-4675-860a-4880ff74cb10" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-eb212d7c-2281-4675-860a-4880ff74cb10" aria-expanded="false" aria-controls="collapse" id="requests-eb212d7c-2281-4675-860a-4880ff74cb10" class="collapsed text-white z-block">
                    Iteration: 1 - PUT category in DB Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-eb212d7c-2281-4675-860a-4880ff74cb10" class="collapse" aria-labelledby="requests-eb212d7c-2281-4675-860a-4880ff74cb10">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> PUT</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/category/add" target="_blank">https://quick-solution.up.railway.app/category/add</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 459ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 92B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar bg-success" style="width: 100%" role="progressbar">
                                            <h5 class="text-uppercase text-white text-center" style="padding-top:5px;"><strong>No Tests for this request</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">a15e9442-0103-4d43-bcde-71febb48df10</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">92</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-0" class="prettyPrint hljs json">{
  <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Seller"</span>,
  <span class="hljs-attr">"logoUrl"</span>: <span class="hljs-string">"https://i.ibb.co/B4yNbZq/Seller.png"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">92</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"5c-ShutYOH895Hqw6kT0TGoGJBY4Q0"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:42 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-c7485f75-eaa1-4372-9efb-5438160130f8" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"modifiedCount"</span>: <span class="hljs-number">0</span>,
  <span class="hljs-attr">"upsertedId"</span>: <span class="hljs-literal">null</span>,
  <span class="hljs-attr">"upsertedCount"</span>: <span class="hljs-number">0</span>,
  <span class="hljs-attr">"matchedCount"</span>: <span class="hljs-number">1</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-c7485f75-eaa1-4372-9efb-5438160130f8">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <h5 class="alert alert-success text-uppercase text-center">No Tests for this request</h5>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-c448daaa-0561-45a6-b598-f261a2b25d44" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-c448daaa-0561-45a6-b598-f261a2b25d44" aria-expanded="false" aria-controls="collapse" id="requests-c448daaa-0561-45a6-b598-f261a2b25d44" class="collapsed text-white z-block">
                    Iteration: 1 - PUT a user to admin Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-c448daaa-0561-45a6-b598-f261a2b25d44" class="collapse" aria-labelledby="requests-c448daaa-0561-45a6-b598-f261a2b25d44">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> PUT</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/user/admin/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/user/admin/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 675ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 92B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">904427de-6c7f-48ad-9a5d-d6182fd23cac</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">0</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">92</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"5c-ShutYOH895Hqw6kT0TGoGJBY4Q0"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:43 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-8a1c3f8d-fd12-4e8b-9d0c-06ed6db5a390" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"modifiedCount"</span>: <span class="hljs-number">0</span>,
  <span class="hljs-attr">"upsertedId"</span>: <span class="hljs-literal">null</span>,
  <span class="hljs-attr">"upsertedCount"</span>: <span class="hljs-number">0</span>,
  <span class="hljs-attr">"matchedCount"</span>: <span class="hljs-number">1</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-8a1c3f8d-fd12-4e8b-9d0c-06ed6db5a390">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_16_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_16_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_16"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_16" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_16" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_16" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_16" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_16" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Admin Maked</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-0f47fa1f-41b5-4bf2-9150-62879b44b8d1-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-0f47fa1f-41b5-4bf2-9150-62879b44b8d1-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Admin users / POST - 1 Request in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-0f47fa1f-41b5-4bf2-9150-62879b44b8d1-iteration-0" class="collapse" aria-labelledby="folder-0f47fa1f-41b5-4bf2-9150-62879b44b8d1" style="border-bottom: none;">
            <div id="folder-62ce75ce-e1a6-489e-855a-a36f7d7b7814" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814" aria-expanded="false" aria-controls="collapse" id="requests-62ce75ce-e1a6-489e-855a-a36f7d7b7814" class="collapsed text-white z-block">
                    Iteration: 1 - POST a review <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814" class="collapse" aria-labelledby="requests-62ce75ce-e1a6-489e-855a-a36f7d7b7814">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/reviews" target="_blank">https://quick-solution.up.railway.app/reviews</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 468ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 61B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar bg-success" style="width: 100%" role="progressbar">
                                            <h5 class="text-uppercase text-white text-center" style="padding-top:5px;"><strong>No Tests for this request</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">25d4399e-6092-4f2b-b9f0-348c6e260115</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">292</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-0" class="prettyPrint hljs json">{
  <span class="hljs-attr">"name"</span>: <span class="hljs-string">"Jamal"</span>,
  <span class="hljs-attr">"img"</span>: <span class="hljs-string">"https://i.ibb.co/dWZ7m3J/photostudio-4-designify.png"</span>,
  <span class="hljs-attr">"email"</span>: <span class="hljs-string">"jamal12@gmail.com"</span>,
  <span class="hljs-attr">"location"</span>: <span class="hljs-string">"Mohammodpur, Dhaka"</span>,
  <span class="hljs-attr">"reviewtext"</span>: <span class="hljs-string">"The site is very useful and good. It a very well designed and decorated."</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">61</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"3d-n3trzkayBqyilPmyfr/cZIcnIb8"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:43 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-b683d4df-1e06-47d1-93ed-8ac39b3b348c" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"insertedId"</span>: <span class="hljs-string">"646ddd7b67d09eadea169a7d"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-b683d4df-1e06-47d1-93ed-8ac39b3b348c">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <h5 class="alert alert-success text-uppercase text-center">No Tests for this request</h5>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        <div class="alert alert-dark text-uppercase text-center iteration-0" style="display: block;">
        <a data-toggle="collapse" href="#" data-target="#folder-collapse-0d65971c-e976-4687-b21c-e7e215125a6b-iteration-0" aria-expanded="false" aria-controls="collapse" id="folder-0d65971c-e976-4687-b21c-e7e215125a6b-iteration-0" class="collapsed text-dark z-block" style="border-bottom: none;">
        <i class="fas fa-info-circle float-left resultsInfoPass"></i>
            Admin users / DELETE - 2 Requests in the folder<i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
        </a>
        </div>
        <div id="folder-collapse-0d65971c-e976-4687-b21c-e7e215125a6b-iteration-0" class="collapse" aria-labelledby="folder-0d65971c-e976-4687-b21c-e7e215125a6b" style="border-bottom: none;">
            <div id="folder-68756c9d-f990-45b3-be96-55eac546f0cd" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-68756c9d-f990-45b3-be96-55eac546f0cd" aria-expanded="false" aria-controls="collapse" id="requests-68756c9d-f990-45b3-be96-55eac546f0cd" class="collapsed text-white z-block">
                    Iteration: 1 - Deleted user from DB Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-68756c9d-f990-45b3-be96-55eac546f0cd" class="collapse" aria-labelledby="requests-68756c9d-f990-45b3-be96-55eac546f0cd">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> DELETE</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com" target="_blank">https://quick-solution.up.railway.app/user/abdullahsayid1218@gmail.com</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 403 - Forbidden</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 243ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 30B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar bg-success" style="width: 100%" role="progressbar">
                                            <h5 class="text-uppercase text-white text-center" style="padding-top:5px;"><strong>No Tests for this request</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">content-type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar token(Which you got from put user API response)</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">8f119dfd-01fa-4a36-bfe7-3cf40f37db4a</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">30</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"1e-NNRZhE06okBNKUTchJtjOZaGRqM"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:44 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-271c4b11-4cbf-41d0-ba79-fc5fb5c0594a" class="prettyPrint hljs json">{
  <span class="hljs-attr">"massage"</span>: <span class="hljs-string">"Forbidden Access"</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-271c4b11-4cbf-41d0-ba79-fc5fb5c0594a">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <h5 class="alert alert-success text-uppercase text-center">No Tests for this request</h5>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-5ca7356d-7677-4ccc-86d7-81f882b6e089" class="card-deck iteration-0" style="display: block;">
            <div class="row iteration-0" style="display: block;">
                <div class="col-sm-12 mb-3 iteration-0" style="display: block;">
                <div class="card iteration-0" style="display: block;">
                    <div class="card-header  bg-success iteration-0" style="display: block;">
                        <a data-toggle="collapse" href="#" data-target="#collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089" aria-expanded="false" aria-controls="collapse" id="requests-5ca7356d-7677-4ccc-86d7-81f882b6e089" class="collapsed text-white z-block">
                    Iteration: 1 - DELETE Review from DB Copy <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089" class="collapse" aria-labelledby="requests-5ca7356d-7677-4ccc-86d7-81f882b6e089">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> DELETE</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="https://quick-solution.up.railway.app/reviews/646ddd7b67d09eadea169a7d" target="_blank">https://quick-solution.up.railway.app/reviews/646ddd7b67d09eadea169a7d</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 463ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 38B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">authorization</td>
                                                        <td class="text-wrap">Bearar eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFiZHVsbGFoc2F5aWQxMjE4QGdtYWlsLmNvbSIsImlhdCI6MTY4NDkyMTcxNiwiZXhwIjoxNjg0OTI1MzE2fQ.hmrZm68H3feLlmgl6MKIzIIQ9vmd4UGzFhrmx4B0chU</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">5d64fdd5-27c7-4d70-b380-b7acb94f601f</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">quick-solution.up.railway.app</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">x-powered-by</td>
                                                    <td class="text-wrap">Express</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">access-control-allow-origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-type</td>
                                                    <td class="text-wrap">application/json; charset=utf-8</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">content-length</td>
                                                    <td class="text-wrap">38</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">etag</td>
                                                    <td class="text-wrap">W/"26-fgR5yLHQ1Hpp6zDESHaY9wJreYE"</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">date</td>
                                                    <td class="text-wrap">Wed, 24 May 2023 09:48:44 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">server</td>
                                                    <td class="text-wrap">railway</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-2e497771-e769-49d2-ac40-1048f435e904" class="prettyPrint hljs json">{
  <span class="hljs-attr">"acknowledged"</span>: <span class="hljs-literal">true</span>,
  <span class="hljs-attr">"deletedCount"</span>: <span class="hljs-number">1</span>
}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-2e497771-e769-49d2-ac40-1048f435e904">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <div id="DataTables_Table_17_wrapper" class="dataTables_wrapper dt-bootstrap4"><div class="row"><div class="col-sm-12 col-md-6"></div><div class="col-sm-12 col-md-6"><div id="DataTables_Table_17_filter" class="dataTables_filter"><label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="DataTables_Table_17"></label></div></div></div><div class="row"><div class="col-sm-12"><table class="datatable table table-hover dataTable" id="DataTables_Table_17" role="grid">
                                        <thead><tr class="text-center" role="row"><th class="sorting_asc" tabindex="0" aria-controls="DataTables_Table_17" rowspan="1" colspan="1" aria-sort="ascending" aria-label="Name: activate to sort column descending" style="width: 0px;">Name</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_17" rowspan="1" colspan="1" aria-label="Passed: activate to sort column ascending" style="width: 0px;">Passed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_17" rowspan="1" colspan="1" aria-label="Failed: activate to sort column ascending" style="width: 0px;">Failed</th><th class="sorting" tabindex="0" aria-controls="DataTables_Table_17" rowspan="1" colspan="1" aria-label="Skipped: activate to sort column ascending" style="width: 0px;">Skipped</th></tr></thead>
                                            <tbody>
                                                
                                            <tr role="row" class="odd">
                                                    <td class="sorting_1">Deleted Review</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr></tbody>
                                            <tfoot>
                                                <tr class="bg-light"><td rowspan="1" colspan="1"><strong>Total</strong></td><td class="text-center" rowspan="1" colspan="1">1</td><td class="text-center" rowspan="1" colspan="1">0</td><td class="text-center" rowspan="1" colspan="1">0</td></tr>
                                            </tfoot>
                                        </table></div></div><div class="row"><div class="col-sm-12 col-md-5"></div><div class="col-sm-12 col-md-7"></div></div></div>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        </div>
    </div>
    </div>
    </div>
    </div>
    </div>


<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.2.1/js/bootstrap.bundle.min.js"></script>
<script src="https://cdn.datatables.net/v/bs4/dt-1.10.18/datatables.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.0/clipboard.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/remarkable/1.7.1/remarkable.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.2/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>

<!-- Set slider initial position depending on the localstorage state -->

<script>
(function () {
  var sliderChecked = true;
  if (localStorage.getItem('theme') === 'theme-light') {
    setTheme('theme-light');
    sliderChecked = false;
  } else {
    setTheme('theme-dark');
    sliderChecked = true;
  }
  $(document).ready( function () {
    document.getElementById('slider').checked = sliderChecked;
  });
})();
</script>

<!-- Data Table Configuration -->

<script>
$(document).ready( function () {
    $('.datatable').DataTable({
        "retrieve": true,
        "paging": false,
        "info": false,
        "fixedColumns":   {
            "heightMatch": 'none'
        }
    });
});
</script>

<!-- Tooltip Configuration -->

<script>
$(document).ready(function() {
    $('[data-toggle="tooltip"]').tooltip({
        trigger : 'hover'
    })
})
</script>

<!-- Show/Hide The Folders -->

<script>
$('#openAll').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
switch (clickCount){
    case 1:
            $('#folder-548b55f1-e86e-4d35-9836-d424a86c359f-iteration-0').removeClass('collapsed')
            $('#folder-collapse-548b55f1-e86e-4d35-9836-d424a86c359f-iteration-0').addClass('show')
            $('#folder-a4369510-7575-47d4-b620-11d381fa3689-iteration-0').removeClass('collapsed')
            $('#folder-collapse-a4369510-7575-47d4-b620-11d381fa3689-iteration-0').addClass('show')
            $('#folder-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81-iteration-0').removeClass('collapsed')
            $('#folder-collapse-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81-iteration-0').addClass('show')
            $('#folder-cd20c794-0e9f-4762-8ce4-997b4cc85feb-iteration-0').removeClass('collapsed')
            $('#folder-collapse-cd20c794-0e9f-4762-8ce4-997b4cc85feb-iteration-0').addClass('show')
            $('#folder-9e323c4a-8667-4374-a10b-2995c7c84562-iteration-0').removeClass('collapsed')
            $('#folder-collapse-9e323c4a-8667-4374-a10b-2995c7c84562-iteration-0').addClass('show')
            $('#folder-6c9a5aa5-57d3-41d7-8de2-9057de500785-iteration-0').removeClass('collapsed')
            $('#folder-collapse-6c9a5aa5-57d3-41d7-8de2-9057de500785-iteration-0').addClass('show')
            $('#folder-0e2a6797-c9e5-43ae-90aa-1f0c1c907830-iteration-0').removeClass('collapsed')
            $('#folder-collapse-0e2a6797-c9e5-43ae-90aa-1f0c1c907830-iteration-0').addClass('show')
            $('#folder-38b8045e-22e4-4ae7-b42a-ba9399265103-iteration-0').removeClass('collapsed')
            $('#folder-collapse-38b8045e-22e4-4ae7-b42a-ba9399265103-iteration-0').addClass('show')
            $('#folder-e807cb85-0182-4073-9d05-a43a0e9cf410-iteration-0').removeClass('collapsed')
            $('#folder-collapse-e807cb85-0182-4073-9d05-a43a0e9cf410-iteration-0').addClass('show')
            $('#folder-0f47fa1f-41b5-4bf2-9150-62879b44b8d1-iteration-0').removeClass('collapsed')
            $('#folder-collapse-0f47fa1f-41b5-4bf2-9150-62879b44b8d1-iteration-0').addClass('show')
            $('#folder-0d65971c-e976-4687-b21c-e7e215125a6b-iteration-0').removeClass('collapsed')
            $('#folder-collapse-0d65971c-e976-4687-b21c-e7e215125a6b-iteration-0').addClass('show')
        $('#openAll').html("Collapse Folders");
        break;
    case 2:
            $('#folder-548b55f1-e86e-4d35-9836-d424a86c359f-iteration-0').addClass('collapsed')
            $('#folder-collapse-548b55f1-e86e-4d35-9836-d424a86c359f-iteration-0').removeClass('show')
            $('#folder-a4369510-7575-47d4-b620-11d381fa3689-iteration-0').addClass('collapsed')
            $('#folder-collapse-a4369510-7575-47d4-b620-11d381fa3689-iteration-0').removeClass('show')
            $('#folder-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81-iteration-0').addClass('collapsed')
            $('#folder-collapse-da32e247-0f31-4ffb-bd0c-cb4dfc37fa81-iteration-0').removeClass('show')
            $('#folder-cd20c794-0e9f-4762-8ce4-997b4cc85feb-iteration-0').addClass('collapsed')
            $('#folder-collapse-cd20c794-0e9f-4762-8ce4-997b4cc85feb-iteration-0').removeClass('show')
            $('#folder-9e323c4a-8667-4374-a10b-2995c7c84562-iteration-0').addClass('collapsed')
            $('#folder-collapse-9e323c4a-8667-4374-a10b-2995c7c84562-iteration-0').removeClass('show')
            $('#folder-6c9a5aa5-57d3-41d7-8de2-9057de500785-iteration-0').addClass('collapsed')
            $('#folder-collapse-6c9a5aa5-57d3-41d7-8de2-9057de500785-iteration-0').removeClass('show')
            $('#folder-0e2a6797-c9e5-43ae-90aa-1f0c1c907830-iteration-0').addClass('collapsed')
            $('#folder-collapse-0e2a6797-c9e5-43ae-90aa-1f0c1c907830-iteration-0').removeClass('show')
            $('#folder-38b8045e-22e4-4ae7-b42a-ba9399265103-iteration-0').addClass('collapsed')
            $('#folder-collapse-38b8045e-22e4-4ae7-b42a-ba9399265103-iteration-0').removeClass('show')
            $('#folder-e807cb85-0182-4073-9d05-a43a0e9cf410-iteration-0').addClass('collapsed')
            $('#folder-collapse-e807cb85-0182-4073-9d05-a43a0e9cf410-iteration-0').removeClass('show')
            $('#folder-0f47fa1f-41b5-4bf2-9150-62879b44b8d1-iteration-0').addClass('collapsed')
            $('#folder-collapse-0f47fa1f-41b5-4bf2-9150-62879b44b8d1-iteration-0').removeClass('show')
            $('#folder-0d65971c-e976-4687-b21c-e7e215125a6b-iteration-0').addClass('collapsed')
            $('#folder-collapse-0d65971c-e976-4687-b21c-e7e215125a6b-iteration-0').removeClass('show')
        $('#openAll').html("Expand Folders");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Show/Hide The Requests -->

<script>
$('#openAllRequests').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
switch (clickCount){
    case 1:
            $('#requests-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('collapsed')
            $('#collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('collapsed')
            $('#requests-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('show')
            $('#collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('show')
            $('#requests-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('collapsed')
            $('#collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('collapsed')
            $('#requests-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('show')
            $('#collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('show')
            $('#requests-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('collapsed')
            $('#collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('collapsed')
            $('#requests-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('show')
            $('#collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('show')
            $('#requests-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('collapsed')
            $('#collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('collapsed')
            $('#requests-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('show')
            $('#collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('show')
            $('#requests-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('collapsed')
            $('#collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('collapsed')
            $('#requests-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('show')
            $('#collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('show')
            $('#requests-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('collapsed')
            $('#collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('collapsed')
            $('#requests-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('show')
            $('#collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('show')
            $('#requests-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('collapsed')
            $('#collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('collapsed')
            $('#requests-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('show')
            $('#collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('show')
            $('#requests-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('collapsed')
            $('#collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('collapsed')
            $('#requests-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('show')
            $('#collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('show')
            $('#requests-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('collapsed')
            $('#collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('collapsed')
            $('#requests-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('show')
            $('#collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('show')
            $('#requests-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('collapsed')
            $('#collapse-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('collapsed')
            $('#requests-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('show')
            $('#collapse-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('show')
            $('#requests-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('collapsed')
            $('#collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('collapsed')
            $('#requests-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('show')
            $('#collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('show')
            $('#requests-b719159f-acfa-479c-9e12-c118ad814145').removeClass('collapsed')
            $('#collapse-b719159f-acfa-479c-9e12-c118ad814145').removeClass('collapsed')
            $('#requests-b719159f-acfa-479c-9e12-c118ad814145').addClass('show')
            $('#collapse-b719159f-acfa-479c-9e12-c118ad814145').addClass('show')
            $('#requests-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('collapsed')
            $('#collapse-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('collapsed')
            $('#requests-fb0e55a3-06db-4273-b951-db7c486363db').addClass('show')
            $('#collapse-fb0e55a3-06db-4273-b951-db7c486363db').addClass('show')
            $('#requests-52b76027-7808-47a8-923b-29d76b54131f').removeClass('collapsed')
            $('#collapse-52b76027-7808-47a8-923b-29d76b54131f').removeClass('collapsed')
            $('#requests-52b76027-7808-47a8-923b-29d76b54131f').addClass('show')
            $('#collapse-52b76027-7808-47a8-923b-29d76b54131f').addClass('show')
            $('#requests-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('collapsed')
            $('#collapse-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('collapsed')
            $('#requests-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('show')
            $('#collapse-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('show')
            $('#requests-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('collapsed')
            $('#collapse-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('collapsed')
            $('#requests-81093223-ad2e-45ab-9d70-655caa29d027').addClass('show')
            $('#collapse-81093223-ad2e-45ab-9d70-655caa29d027').addClass('show')
            $('#requests-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('collapsed')
            $('#collapse-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('collapsed')
            $('#requests-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('show')
            $('#collapse-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('show')
            $('#requests-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('collapsed')
            $('#collapse-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('collapsed')
            $('#requests-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('show')
            $('#collapse-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('show')
            $('#requests-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('collapsed')
            $('#collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('collapsed')
            $('#requests-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('show')
            $('#collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('show')
            $('#requests-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('collapsed')
            $('#collapse-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('collapsed')
            $('#requests-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('show')
            $('#collapse-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('show')
            $('#requests-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('collapsed')
            $('#collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('collapsed')
            $('#requests-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('show')
            $('#collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('show')
        $('#openAllRequests').html("Collapse Requests");
        break;
    case 2:
            $('#requests-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('collapsed')
            $('#collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('collapsed')
            $('#requests-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('show')
            $('#collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('show')
            $('#requests-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('collapsed')
            $('#collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('collapsed')
            $('#requests-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('show')
            $('#collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('show')
            $('#requests-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('collapsed')
            $('#collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('collapsed')
            $('#requests-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('show')
            $('#collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('show')
            $('#requests-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('collapsed')
            $('#collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('collapsed')
            $('#requests-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('show')
            $('#collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('show')
            $('#requests-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('collapsed')
            $('#collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('collapsed')
            $('#requests-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('show')
            $('#collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('show')
            $('#requests-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('collapsed')
            $('#collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('collapsed')
            $('#requests-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('show')
            $('#collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('show')
            $('#requests-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('collapsed')
            $('#collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('collapsed')
            $('#requests-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('show')
            $('#collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('show')
            $('#requests-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('collapsed')
            $('#collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('collapsed')
            $('#requests-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('show')
            $('#collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('show')
            $('#requests-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('collapsed')
            $('#collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('collapsed')
            $('#requests-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('show')
            $('#collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('show')
            $('#requests-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('collapsed')
            $('#collapse-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('collapsed')
            $('#requests-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('show')
            $('#collapse-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('show')
            $('#requests-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('collapsed')
            $('#collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('collapsed')
            $('#requests-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('show')
            $('#collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('show')
            $('#requests-b719159f-acfa-479c-9e12-c118ad814145').addClass('collapsed')
            $('#collapse-b719159f-acfa-479c-9e12-c118ad814145').addClass('collapsed')
            $('#requests-b719159f-acfa-479c-9e12-c118ad814145').removeClass('show')
            $('#collapse-b719159f-acfa-479c-9e12-c118ad814145').removeClass('show')
            $('#requests-fb0e55a3-06db-4273-b951-db7c486363db').addClass('collapsed')
            $('#collapse-fb0e55a3-06db-4273-b951-db7c486363db').addClass('collapsed')
            $('#requests-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('show')
            $('#collapse-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('show')
            $('#requests-52b76027-7808-47a8-923b-29d76b54131f').addClass('collapsed')
            $('#collapse-52b76027-7808-47a8-923b-29d76b54131f').addClass('collapsed')
            $('#requests-52b76027-7808-47a8-923b-29d76b54131f').removeClass('show')
            $('#collapse-52b76027-7808-47a8-923b-29d76b54131f').removeClass('show')
            $('#requests-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('collapsed')
            $('#collapse-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('collapsed')
            $('#requests-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('show')
            $('#collapse-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('show')
            $('#requests-81093223-ad2e-45ab-9d70-655caa29d027').addClass('collapsed')
            $('#collapse-81093223-ad2e-45ab-9d70-655caa29d027').addClass('collapsed')
            $('#requests-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('show')
            $('#collapse-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('show')
            $('#requests-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('collapsed')
            $('#collapse-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('collapsed')
            $('#requests-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('show')
            $('#collapse-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('show')
            $('#requests-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('collapsed')
            $('#collapse-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('collapsed')
            $('#requests-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('show')
            $('#collapse-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('show')
            $('#requests-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('collapsed')
            $('#collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('collapsed')
            $('#requests-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('show')
            $('#collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('show')
            $('#requests-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('collapsed')
            $('#collapse-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('collapsed')
            $('#requests-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('show')
            $('#collapse-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('show')
            $('#requests-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('collapsed')
            $('#collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('collapsed')
            $('#requests-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('show')
            $('#collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('show')
        $('#openAllRequests').html("Expand Requests");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Show/Hide The Skipped Tests -->

<script>
$('#openAllSkipped').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
switch (clickCount){
    case 1:
            $('#skipped-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('collapsed')
            $('#skipped-collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('collapsed')
            $('#skipped-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('show')
            $('#skipped-collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('show')
            $('#skipped-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('collapsed')
            $('#skipped-collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('collapsed')
            $('#skipped-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('show')
            $('#skipped-collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('show')
            $('#skipped-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('collapsed')
            $('#skipped-collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('collapsed')
            $('#skipped-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('show')
            $('#skipped-collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('show')
            $('#skipped-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('collapsed')
            $('#skipped-collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('collapsed')
            $('#skipped-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('show')
            $('#skipped-collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('show')
            $('#skipped-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('collapsed')
            $('#skipped-collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('collapsed')
            $('#skipped-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('show')
            $('#skipped-collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('show')
            $('#skipped-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('collapsed')
            $('#skipped-collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('collapsed')
            $('#skipped-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('show')
            $('#skipped-collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('show')
            $('#skipped-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('collapsed')
            $('#skipped-collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('collapsed')
            $('#skipped-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('show')
            $('#skipped-collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('show')
            $('#skipped-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('collapsed')
            $('#skipped-collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('collapsed')
            $('#skipped-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('show')
            $('#skipped-collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('show')
            $('#skipped-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('collapsed')
            $('#skipped-collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('collapsed')
            $('#skipped-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('show')
            $('#skipped-collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('show')
            $('#skipped-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('collapsed')
            $('#skipped-collapse-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('collapsed')
            $('#skipped-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('show')
            $('#skipped-collapse-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('show')
            $('#skipped-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('collapsed')
            $('#skipped-collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('collapsed')
            $('#skipped-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('show')
            $('#skipped-collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('show')
            $('#skipped-b719159f-acfa-479c-9e12-c118ad814145').removeClass('collapsed')
            $('#skipped-collapse-b719159f-acfa-479c-9e12-c118ad814145').removeClass('collapsed')
            $('#skipped-b719159f-acfa-479c-9e12-c118ad814145').addClass('show')
            $('#skipped-collapse-b719159f-acfa-479c-9e12-c118ad814145').addClass('show')
            $('#skipped-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('collapsed')
            $('#skipped-collapse-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('collapsed')
            $('#skipped-fb0e55a3-06db-4273-b951-db7c486363db').addClass('show')
            $('#skipped-collapse-fb0e55a3-06db-4273-b951-db7c486363db').addClass('show')
            $('#skipped-52b76027-7808-47a8-923b-29d76b54131f').removeClass('collapsed')
            $('#skipped-collapse-52b76027-7808-47a8-923b-29d76b54131f').removeClass('collapsed')
            $('#skipped-52b76027-7808-47a8-923b-29d76b54131f').addClass('show')
            $('#skipped-collapse-52b76027-7808-47a8-923b-29d76b54131f').addClass('show')
            $('#skipped-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('collapsed')
            $('#skipped-collapse-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('collapsed')
            $('#skipped-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('show')
            $('#skipped-collapse-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('show')
            $('#skipped-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('collapsed')
            $('#skipped-collapse-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('collapsed')
            $('#skipped-81093223-ad2e-45ab-9d70-655caa29d027').addClass('show')
            $('#skipped-collapse-81093223-ad2e-45ab-9d70-655caa29d027').addClass('show')
            $('#skipped-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('collapsed')
            $('#skipped-collapse-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('collapsed')
            $('#skipped-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('show')
            $('#skipped-collapse-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('show')
            $('#skipped-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('collapsed')
            $('#skipped-collapse-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('collapsed')
            $('#skipped-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('show')
            $('#skipped-collapse-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('show')
            $('#skipped-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('collapsed')
            $('#skipped-collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('collapsed')
            $('#skipped-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('show')
            $('#skipped-collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('show')
            $('#skipped-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('collapsed')
            $('#skipped-collapse-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('collapsed')
            $('#skipped-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('show')
            $('#skipped-collapse-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('show')
            $('#skipped-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('collapsed')
            $('#skipped-collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('collapsed')
            $('#skipped-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('show')
            $('#skipped-collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('show')
        $('#openAllSkipped').html("Collapse All Skipped Tests");
        break;
    case 2:
            $('#skipped-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('collapsed')
            $('#skipped-collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').addClass('collapsed')
            $('#skipped-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('show')
            $('#skipped-collapse-b8e0aae1-7bf3-42af-9c7d-e544c7acc06e').removeClass('show')
            $('#skipped-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('collapsed')
            $('#skipped-collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').addClass('collapsed')
            $('#skipped-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('show')
            $('#skipped-collapse-eeba57cd-d08a-4da5-bb40-2866f6d2a63c').removeClass('show')
            $('#skipped-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('collapsed')
            $('#skipped-collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').addClass('collapsed')
            $('#skipped-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('show')
            $('#skipped-collapse-5f404d88-02a6-43fd-aaeb-ed09f694cff0').removeClass('show')
            $('#skipped-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('collapsed')
            $('#skipped-collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').addClass('collapsed')
            $('#skipped-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('show')
            $('#skipped-collapse-eddc7c2e-4a44-43a8-b6e3-233c57a21529').removeClass('show')
            $('#skipped-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('collapsed')
            $('#skipped-collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').addClass('collapsed')
            $('#skipped-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('show')
            $('#skipped-collapse-75f7c382-c313-4d8a-9ad0-27f8231d725e').removeClass('show')
            $('#skipped-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('collapsed')
            $('#skipped-collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').addClass('collapsed')
            $('#skipped-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('show')
            $('#skipped-collapse-73445db5-8e9d-4b11-b3f1-3314169e173b').removeClass('show')
            $('#skipped-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('collapsed')
            $('#skipped-collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').addClass('collapsed')
            $('#skipped-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('show')
            $('#skipped-collapse-07bf8973-f568-4e38-8cff-9634f5a27ac3').removeClass('show')
            $('#skipped-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('collapsed')
            $('#skipped-collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').addClass('collapsed')
            $('#skipped-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('show')
            $('#skipped-collapse-2fdd34c5-2fda-4077-b0aa-208aa5d7cee9').removeClass('show')
            $('#skipped-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('collapsed')
            $('#skipped-collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').addClass('collapsed')
            $('#skipped-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('show')
            $('#skipped-collapse-3a7ced69-9d5c-42bb-a382-962812c5ade3').removeClass('show')
            $('#skipped-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('collapsed')
            $('#skipped-collapse-6c86f601-cf57-41ee-9144-beeeb611895c').addClass('collapsed')
            $('#skipped-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('show')
            $('#skipped-collapse-6c86f601-cf57-41ee-9144-beeeb611895c').removeClass('show')
            $('#skipped-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('collapsed')
            $('#skipped-collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').addClass('collapsed')
            $('#skipped-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('show')
            $('#skipped-collapse-eced55c6-6fc9-413c-91b7-c0a3e40d190e').removeClass('show')
            $('#skipped-b719159f-acfa-479c-9e12-c118ad814145').addClass('collapsed')
            $('#skipped-collapse-b719159f-acfa-479c-9e12-c118ad814145').addClass('collapsed')
            $('#skipped-b719159f-acfa-479c-9e12-c118ad814145').removeClass('show')
            $('#skipped-collapse-b719159f-acfa-479c-9e12-c118ad814145').removeClass('show')
            $('#skipped-fb0e55a3-06db-4273-b951-db7c486363db').addClass('collapsed')
            $('#skipped-collapse-fb0e55a3-06db-4273-b951-db7c486363db').addClass('collapsed')
            $('#skipped-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('show')
            $('#skipped-collapse-fb0e55a3-06db-4273-b951-db7c486363db').removeClass('show')
            $('#skipped-52b76027-7808-47a8-923b-29d76b54131f').addClass('collapsed')
            $('#skipped-collapse-52b76027-7808-47a8-923b-29d76b54131f').addClass('collapsed')
            $('#skipped-52b76027-7808-47a8-923b-29d76b54131f').removeClass('show')
            $('#skipped-collapse-52b76027-7808-47a8-923b-29d76b54131f').removeClass('show')
            $('#skipped-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('collapsed')
            $('#skipped-collapse-8b8ac03a-f031-4422-850f-10c74b16f072').addClass('collapsed')
            $('#skipped-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('show')
            $('#skipped-collapse-8b8ac03a-f031-4422-850f-10c74b16f072').removeClass('show')
            $('#skipped-81093223-ad2e-45ab-9d70-655caa29d027').addClass('collapsed')
            $('#skipped-collapse-81093223-ad2e-45ab-9d70-655caa29d027').addClass('collapsed')
            $('#skipped-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('show')
            $('#skipped-collapse-81093223-ad2e-45ab-9d70-655caa29d027').removeClass('show')
            $('#skipped-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('collapsed')
            $('#skipped-collapse-eb212d7c-2281-4675-860a-4880ff74cb10').addClass('collapsed')
            $('#skipped-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('show')
            $('#skipped-collapse-eb212d7c-2281-4675-860a-4880ff74cb10').removeClass('show')
            $('#skipped-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('collapsed')
            $('#skipped-collapse-c448daaa-0561-45a6-b598-f261a2b25d44').addClass('collapsed')
            $('#skipped-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('show')
            $('#skipped-collapse-c448daaa-0561-45a6-b598-f261a2b25d44').removeClass('show')
            $('#skipped-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('collapsed')
            $('#skipped-collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').addClass('collapsed')
            $('#skipped-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('show')
            $('#skipped-collapse-62ce75ce-e1a6-489e-855a-a36f7d7b7814').removeClass('show')
            $('#skipped-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('collapsed')
            $('#skipped-collapse-68756c9d-f990-45b3-be96-55eac546f0cd').addClass('collapsed')
            $('#skipped-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('show')
            $('#skipped-collapse-68756c9d-f990-45b3-be96-55eac546f0cd').removeClass('show')
            $('#skipped-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('collapsed')
            $('#skipped-collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').addClass('collapsed')
            $('#skipped-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('show')
            $('#skipped-collapse-5ca7356d-7677-4ccc-86d7-81f882b6e089').removeClass('show')
        $('#openAllSkipped').html("Expand All Skipped Tests");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Show/Hide The Failures -->

<script>
$('#openAllFailed').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
let failedItemContent
let failedItemHeading
switch (clickCount){
    case 1:
        $('#openAllFailed').html("Collapse All Failed Tests");
        break;
    case 2:
        $('#openAllFailed').html("Expand All Failed Tests");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Pretty Print the Response Body-->

<script>
function isJSON(data)
{
    var ret = true;
    try {
            JSON.parse(data);
    }catch(e) {
            ret = false;
    }
    return ret;
}

function isXML(data)
{
    return (data.length > 0 && data[0] === '<');
}

// see https://gist.github.com/sente/1083506/d2834134cd070dbcc08bf42ee27dabb746a1c54d#gistcomment-2254622
function formatXML(data) {
    const PADDING = ' '.repeat(2); // set desired indent size here
    const reg = /(>)(<)(\/*)/g;
    let pad = 0;
    xml = data.replace(reg, '$1\r\n$2$3');

    return xml.split('\r\n').map((node, index) => {
        let indent = 0;
        if (node.match(/.+<\/\w[^>]*>$/)) {
            indent = 0;
        } else if (node.match(/^<\/\w/) && pad > 0) {
            pad -= 1;
        } else if (node.match(/^<\w[^>]*[^\/]>.*$/)) {
            indent = 1;
        } else {
            indent = 0;
        }

        pad += indent;
        return PADDING.repeat(pad - indent) + node;
    }).join('\r\n');
}

$(".prettyPrint").each(function () {
        var data = $(this).text();
        // Verify whether data is JSON
        if(isJSON(data))
        {
                obj = JSON.parse(data);
                data = JSON.stringify(obj, null, 2);
        }
        else if(isXML(data)) {
            data = formatXML(data);
        }
        $(this).text(data);
});
</script>


<!-- Copy Response Body To Clipboard -->

<script>
    var clipboard = new ClipboardJS('.copyButton');

    clipboard.on('success', function(e) {
        e.clearSelection();
        $(".copyButton").addClass("bg-success text-white")
        e.trigger.textContent = '✔ Copied!';
        window.setTimeout(function() {
            $(".copyButton").removeClass("bg-success text-white")
            e.trigger.textContent = 'Copy to Clipboard';
        }, 2000);
    });
    clipboard.on('error', function(e) {
        e.clearSelection();
        $(".copyButton").addClass("bg-danger text-white")
        e.trigger.textContent = '✗ Not Copied';
        window.setTimeout(function() {
            $(".copyButton").removeClass("bg-danger text-white")
            e.trigger.textContent = 'Copy to Clipboard';
        }, 2000);
    });

</script>

<!-- Render the Description Markdown and link in the test failures -->

<script>
    const remarkable = new Remarkable();

    const descriptions = document.querySelectorAll(".renderMarkdown");
    descriptions.forEach(description => {
        description.innerHTML = renderHtmlFromMarkdown(description.textContent);
    });
    function renderHtmlFromMarkdown(markdown) {
        return remarkable.render(trim(markdown));
    }
    function trim(string) {
        return string ? string.replace(/^ +| +$/gm, "") : string;
    }
</script>

<!-- Show/Hide The Toggles When Scrolling The Page -->

<script>
window.onscroll = function() {scrollFunction()};

function scrollFunction() {
  if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
    document.getElementById("topOfRequestsScreen").style.display = "block";
    document.getElementById("topOfFailuresScreen").style.display = "block";
    document.getElementById("topOfSkippedScreen").style.display = "block";
    document.getElementById("openAll").style.display = "none";
    document.getElementById("openAllRequests").style.display = "none";


  } else {
    document.getElementById("topOfRequestsScreen").style.display = "none";
    document.getElementById("topOfFailuresScreen").style.display = "none";
    document.getElementById("topOfSkippedScreen").style.display = "none";
    document.getElementById("openAll").style.display = "block";
    document.getElementById("openAllRequests").style.display = "block";

  }
}

function topFunction() {
  document.body.scrollTop = 0;
  document.documentElement.scrollTop = 0;
}
</script>

<!-- Creates The Iteration Tabs -->

<script type="text/javascript">
    "use strict";

window.onload = function () {

  // set display for all blocks of response
  var allItems = document.querySelectorAll('[class*=iteration-]');
  allItems.forEach(function(elem){
    elem.style.display = 'block';
  });

   
  let totalIterations = 1;
   

  let menu = document.querySelector('#execution-menu .nav');

  for(var i = 0; i < totalIterations; i++)
  {
    let li = document.createElement('li');
    li.appendChild(document.createTextNode((i + 1)));
    li.setAttribute('id', 'iteration-' + i);
    li.classList.add("custom-tab");
    li.classList.add("itPassed");

    li.addEventListener('click', function() {
      //set display to none for all except row
      let allItems = document.querySelectorAll('[class*=iteration-]:not(.row)');
      allItems.forEach(function(elem) {
        elem.style.display = 'none';
      })

      let allMenus = document.querySelectorAll('[id*=iteration-]');
      allMenus.forEach(function(elem){
        elem.style.borderBottom = 'none';
      })

      this.style.borderBottom = 'solid 3px #032a33';

      let items = document.querySelectorAll("." + this.id + ':not(.row)');
      items.forEach(function(elem) {
        elem.style.display = elem.style.display == 'block' ? 'none' : 'block';
      })
    });
    menu.appendChild(li);
  }

  //shows first tab data
  document.getElementById('iteration-0').click();
  document.getElementById('iterationSelected').innerHTML = `Iteration ${document.getElementById('iteration-0').innerHTML} selected`

}
</script>

<!-- Create the Selected Iteration Label -->

<script>
$(document).ready(function(){
    $(function() {
        $("#iterationList li").click(function() {
            document.getElementById('iterationSelected').innerHTML = "Iteration " + this.innerHTML + " selected"
        });
    });
});
</script>

<!-- Filter Action for the Iterations -->

<script>
$("#filterInput").on("input paste", function() {
    var value = $(this).val();
    $("#iterationList li").filter(function() {
	    $("#showOnlyFailures").data("clickCount") ? $("#showOnlyFailures").click():null;
        $(this).toggle($(this).text().indexOf(value) > -1)
    });
});
</script>

<!-- Showing the Failed Interations -->

<script>
$('#showOnlyFailures').on('click', function(e) {
    let clickCount = $(this).data("clickCount") || 1
	$("#filterInput").val()!="" && clickCount==1 ? $("#filterInput").val('').trigger('input'): null;
    let selectedIteration = $('#iterationList li').filter(function () {
        return $(this).css('border-bottom').indexOf("solid") > -1 && $(this).hasClass('itFailed');
    });
    selectedIteration.length || clickCount > 1 ? null : $("#iterationList li.itFailed")[0].click()
    $("#iterationList li.itPassed").toggle()
    $("div.bg-success [id*=requests]").parents('[class^="row iteration-"]').toggle();
    clickCount = clickCount > 1 ? 1 : ++clickCount;
    clickCount > 1 ? $("#showOnlyFailures").html("Show All Iterations") : $("#showOnlyFailures").html("Show Failed Iterations");
    $(this).data("clickCount", clickCount)
})
</script>


</body>
