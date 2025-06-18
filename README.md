 

# 📁 No_Mask_Detector(N.M.D)
## 🐸 Mask Detection Project 🐸
Final capstone project of the PlayData Pose-Estimation Developer Training Program - "N.M.D"
<br><br>
A system that uses a deep learning model to detect mask usage and identifies unmasked individuals using a Face Identification API, assigning penalties accordingly.
<br>

## 👩‍💻 Team Members
#### • 🧑🏻‍ Sungwoo Park (Team Leader, ML & Frontend) : Developed deep learning model, app, and managed the project
#### • 👩🏻‍🦰 Chaeyeon Park (Frontend) : Developed Admin page, handled web-server communication (Node.js), contributed to backend
#### • 🧑🏻 Byunghun Lee (Frontend) : Developed Admin page, web-server communication (Node.js), backend, and Face Identification
#### • 👩🏻 Joohyun Park (Backend) : Built AWS server, database, and developed iOS app
#### • 👩🏻 Kieun Nam (Backend) : Worked on Face Identification
<br>

## 📚 Project Overview
### <strong>Purpose<br> </strong>
With mandatory mask policies due to the spread of COVID-19, the societal cost of monitoring mask usage indoors has increased. This project aims to reduce such costs by promoting mask compliance within groups using deep learning-based detection and a penalty system.
<br><br>

## Requirements
 - Core Features:
   - iOS app functionality
   - Detects mask presence
   - Validates correct mask usage
   - Identifies and assigns penalty to unmasked individuals via face recognition
   
 - Additional Features:
   - Admin dashboard for managing users
   - User dashboard for viewing personal penalty history
   
 ### iOS Application API Documentation
 ![Screen Shot 2020-12-04 at 1 11 58 PM](https://user-images.githubusercontent.com/64248514/101120975-4f33ed80-3632-11eb-9669-3ffe935b02d5.png)
 ![Screen Shot 2020-12-05 at 11 16 33 PM](https://user-images.githubusercontent.com/64248514/101245772-8d283300-3752-11eb-9743-82b0e51f6d66.png)

## Development Summary
  - Deep Learning: Model selection, data preprocessing, training, and conversion for iOS deployment

  - iOS App: Development, DB connectivity, input format handling

  - Backend/DB: Environment setup, DB architecture design

## 📝 Tech Stack
![Generic badge](https://img.shields.io/badge/platform-Web/iOS-brightgreen.svg) 
![Generic badge](https://img.shields.io/badge/framework-tensorflow/React-green.svg)
![Generic badge](https://img.shields.io/badge/engine-node.js-green.svg)
![Generic badge](https://img.shields.io/badge/database-MySQL-yellow.svg) 
![Generic badge](https://img.shields.io/badge/api-FaceAPI/MobileNetV2-red,.svg) 
![Generic badge](https://img.shields.io/badge/language-Python,JavaScript-important.svg) 
![Generic badge](https://img.shields.io/badge/server-AWS-important.svg)
<br>

## 💻 Prototypes
### Mobile 
![prototype 001](https://user-images.githubusercontent.com/64248514/99365157-40430080-28fa-11eb-8f9f-e5dddd378f9e.jpeg)
### Admin Web Dashboard
![prototype 002](https://user-images.githubusercontent.com/64248514/99365170-43d68780-28fa-11eb-8152-1e61b1e8e90d.jpeg)


## 🦴 System Overview
![전체개요](https://user-images.githubusercontent.com/61309080/100186214-f032f200-2f28-11eb-9bc0-691c4d21718e.jpeg)

![Screen Shot 2020-12-04 at 1 12 50 AM](https://github.com/user-attachments/assets/939e8792-82b9-46d8-bf10-d8f43686d639)

![Screen Shot 2020-12-04 at 1 11 56 AM](https://github.com/user-attachments/assets/6fc92a34-42e5-4379-8ff5-3e250d2edb9b)

- 원본 편집 주소   
https://o365uos-my.sharepoint.com/:x:/g/personal/2016440050_office_uos_ac_kr/EZ1ecBsRLGBHlej1hgj58UAB_hGtvV6s7FHVLKtI6wEwyQ?e=wN0XZh 

<hr> 

### Technical Details
| Technology | Version | Description |
| :--------: | :----: | ---- |
| REST API | ![Generic badge](https://img.shields.io/badge/release--blue.svg) | Complies with REST architectural constraints |
| MVC Pattern | ![Generic badge](https://img.shields.io/badge/release--blue.svg) | Separates application into Model, View, Controller |
| ESLint | ![Generic badge](https://img.shields.io/badge/release-6.14.8-blue.svg) | Linter for ECMAScript/JavaScript code |
| Node.js Express | ![Generic badge](https://img.shields.io/badge/release-6.14.8-blue.svg) | Backend framework |
| React-Admin | ![Generic badge](https://img.shields.io/badge/release-6.14.8-blue.svg) | Admin interface with React |
| Keras | ![Generic badge](https://img.shields.io/badge/release-6.14.8-blue.svg) | Deep learning API in Python |
| MySQL | ![Generic badge](https://img.shields.io/badge/release-6.14.8-blue.svg) | Relational database system |
| CoreML | ![Generic badge](https://img.shields.io/badge/release-6.14.8-blue.svg) | Apple's machine learning framework for iOS |
| X-Code | ![Generic badge](https://img.shields.io/badge/release-6.14.8-blue.svg) | IDE for iOS/macOS development |

<br>

## 📜 ERD (Entity Relationship Diagram)
![Screen Shot 2020-12-08 at 9 22 49 AM](https://user-images.githubusercontent.com/64248514/101421241-3af43700-3937-11eb-918d-6f06f501af8f.png)
<br>

| Entity | Attributes | Domains | DataType |
| :------: | ---------- | ------- | ------ |
| MEMBER | MEM_NO <br> MEM_NAME <br> MEM_COUNT <br> MEM_FACE | ID(PK) <br> Name <br> Penalty Count <br> Face Image URL | INT <br> VARCHAR(45) <br> INT <br> VARCHAR(100) |
| STATE | ST_NO <br> ST_MEM_NO <br> ST_TIME <br> ST_NOTE | Log ID(PK) <br> Member FK(FK) <br> Time <br> Note | INT <br> INT <br> DATETIME <br> VARCHAR(100) | 
| ADMIN | ADMIN_NO <br> ADMIN_ID <br> ADMIN_PW <br> ADMIN_TEL | ID(PK) <br> Username <br> Password <br> Phone Number | INT <br> VARCHAR(45) <br> VARCHAR(45) <br> VARCHAR(45) |

<br><br>

## 🔎 Project Structure

| FrontEnd | BackEnd (main)| BackEnd (test) |
| -------- | ------------- | -------------- |
| ![Screen Shot 2020-10-11 at 9 49 34 PM](https://user-images.githubusercontent.com/64248514/95679127-b2de0380-0c0b-11eb-8a49-c50b1fd676d6.png) | ![Screen Shot 2020-10-11 at 9 44 55 PM](https://user-images.githubusercontent.com/64248514/95679002-1287df00-0c0b-11eb-8141-1c0bd3e5e787.png) | ![Screen Shot 2020-10-11 at 9 25 22 PM](https://user-images.githubusercontent.com/64248514/95678607-b1f7a280-0c08-11eb-8d2c-2856b91e2210.png) |

<br>

# Implemented Features
  - 
  
# BackEnd API url document
  - Common Field
      - Get an image : /member/faceImages/:imageName, GET
          - return : single image data
      - Log-in : /login, POST
          - return : single admin object
          
  - Member Entity
      - Read all : /member, GET
          - return : all of member objects
      - Create one member : /member, POST
          - return : single member object
          - input image multer key : "memberFace"
      - Update one member : /member/:memberId, PUT
          - return : single member object
          - input image multer key : "updateMemberFace"
      - Delete one member : /member/:memberId, DELETE
          - return : boolean
      - Get one member : /member/:memberId, GET
          - return : single member object
          
   - State Entity
      - Read all : /state, GET
          - return : all of state objects
      - Create one state : /state, POST
          - return : single state object
      - Update one state : /state/:stateId, PUT
          - return : single state object
      - Delete one state : /state/:stateId, DELETE
          - return : boolean
      - Get one state : /state/:stateId, GET
          - return : single state object
          
   - Admin Entity
      - Read all : /admin, GET
          - return : all of admin objects
      - Create one admin : /admin, POST
          - return : single admin object
      - Update one admin : /admin/:adminId, PUT
          - return : single admin object
      - Delete one admin : /admin/:adminId, DELETE
          - return : boolean
      - Get one admin : /admin/:adminId, GET
          - return : single admin object
          
   - iOS
      - Image recognition & penalty : /nomask, POST
          - return : {"result" : "true", "username" : member's name, "count" : penalty count , "eDistance" : euclidean distance from reference picture descriptor } 
                      || { "result": "false", "username" : "unknown", "eDistance" : euclidean distance over 0.6 }
          - input image multer key : "tempFace"
      - Warning admin : /call, GET
          - return :  true || false
 
# Repositories by Feature
  - React-admin&React : https://github.com/byungs2/DeepLearningProjectFrontEnd
  - Node.js Express&Sequelize : https://github.com/byungs2/DeepLearningProjectBackEnd
  - Deep learning model and training : https://github.com/simonpark90/mask_deeplearning
  - face-api.js : https://github.com/pure-teatree/FaceApi_Test
  - Swift x React x Node.js express x MySQL : https://github.com/j00hyun/iOS-React-App
