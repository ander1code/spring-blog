# 🌱 Spring-Blog

![Programming Language](https://img.shields.io/badge/Java-red?style=flat&logo=openjdk&logoColor=white)
![Framework](https://img.shields.io/badge/Spring%20Framework-green?style=flat&logo=spring&logoColor=white)
![Frontend Framework](https://img.shields.io/badge/AngularJS-darkred?style=flat&logo=angular&logoColor=white)
![Library](https://img.shields.io/badge/jQuery-blue?style=flat&logo=jquery&logoColor=white)
![CSS Framework](https://img.shields.io/badge/Bootstrap-purple?style=flat&logo=bootstrap&logoColor=white)

![Database](https://img.shields.io/badge/PostgreSQL-darkblue?style=flat&logo=postgresql&logoColor=white)
![ORM](https://img.shields.io/badge/Hibernate-beige?style=flat&logo=hibernate&logoColor=white)

![Platform: Web](https://img.shields.io/badge/Platform-Web-blue?style=flat&logo=google-chrome)
![Last Commit](https://img.shields.io/github/last-commit/ander1code/spring-blog?color=yellow&logo=github)

---

## 📝 1. Description
**Spring-Blog** is a dynamic blog application originally developed in **2018**, using older versions of **Java**, the **Spring Framework**, and **Hibernate ORM** for database integration with **PostgreSQL**.  
The front-end is built with **AngularJS** and **jQuery**, providing a responsive and interactive user experience.

---

## ⚙️ 2. Features
- 👤 **Author-Specific Posts:** Each post can only be created, edited, or deleted by its respective author.  
- 🔒 **Role-Based Restrictions:** Users cannot modify or delete posts created by other authors.  
- 📄 **Pagination:** Displays paginated posts for better navigation and usability.

---

## 🧰 3. Tools and Technologies

### 🧩 3.1. Template
- 🎨 **Clean Blog Theme:** Based on **Bootstrap 4**, sourced from [StartBootstrap](https://startbootstrap.com/template-overviews/clean-blog/).

### ☕ 3.2. Java Version
- **Java 1.8 (JDK 1.8.0_161):** Used for building and running the back-end application.

### 🌿 3.3. Web Framework
- **Spring Framework 4.0.1.RELEASE:** Provides a robust and scalable foundation for the server-side logic.

### 💻 3.4. JavaScript Frameworks
- **AngularJS 1.6.9:** For creating dynamic and responsive front-end components.  
- **jQuery 3.3.1:** For efficient DOM manipulation and event handling.

#### 🔧 3.4.1. JavaScript Add-ons
- 🧮 **Pagination:**  
  - `jQuery DataTables` for managing tabular data with pagination.  
- 📁 **File Uploads:**  
  - `ng-file-upload` (v12.2.13)  
  - `ng-file-upload-shim` (v12.2.13)

### 🗄️ 3.5. ORM Framework
- **Hibernate ORM 4.3.1.Final:** Manages database operations and maps Java objects to relational data.

### 🐘 3.6. Database Driver
- **PostgreSQL Driver 9.4.1209.jre7:** Handles database connectivity.

### 📦 3.7. Dependencies

#### 🔄 3.7.1. JSON Conversion
- **Gson 2.8.2:** For converting Java objects to and from JSON.

#### 📂 3.7.2. File Upload
- **Apache Commons FileUpload**, **Commons IO**, and **Commons Codec**: Used for handling file uploads and I/O operations.

### 🧠 3.8. IDE
- **NetBeans IDE 8.2:** Used for development and debugging.

---

## 🚀 Optional Improvements
- 🧭 Add a **Getting Started** section with setup and run instructions.  
- 🖼️ Include **screenshots** or **GIFs** of the interface.  
- ⚖️ Add a **License** section (e.g., MIT License).  
- 📬 Provide **contact** or **contributor information**.

---

### 📁 A. Folder Structure:

📦 Spring-Blog
├── 📄 nb-configuration.xml
├── 📄 pom.xml
├── 📄 README.md
│
└── 📂 src
    └── 📂 main
        ├── 📂 java
        │   └── 📂 com/springblog
        │       ├── 📂 controllers
        │       │   ├── 📄 AppController.java
        │       │   ├── 📄 LoginController.java
        │       │   └── 📄 PostController.java
        │       │
        │       ├── 📂 dtos
        │       │   └── 📄 PostDTO.java
        │       │
        │       ├── 📂 models
        │       │   ├── 📄 Author.java
        │       │   ├── 📄 Post.java
        │       │   └── 📄 UserSys.java
        │       │
        │       └── 📂 services
        │           ├── 📂 connections
        │           │   └── 📄 ConnectionSession.java
        │           │
        │           ├── 📂 daos
        │           │   ├── 📄 AuthorDAO.java
        │           │   ├── 📄 PostDAO.java
        │           │   └── 📄 UserDAO.java
        │           │
        │           ├── 📂 functions
        │           │   ├── 📄 Alert.java
        │           │   ├── 📄 ErrorClass.java
        │           │   ├── 📄 Picture.java
        │           │   └── 📄 ValidationData.java
        │           │
        │           └── 📂 security
        │               ├── 📄 AuthorizerInterceptor.java
        │               ├── 📄 Hash.java
        │               └── 📄 Token.java
        │
        ├── 📂 resources
        │   └── 📄 hibernate.cfg.xml
        │
        └── 📂 webapp
            ├── 📄 redirect.jsp
            │
            ├── 📂 META-INF
            │   └── 📄 context.xml
            │
            ├── 📂 resources
            │   ├── 📂 css
            │   │   ├── 📂 styles
            │   │   │   ├── 📄 form.css
            │   │   │   ├── 📄 index.css
            │   │   │   └── 📄 login.css
            │   │   │
            │   │   └── 📂 vendor
            │   │       ├── 📄 bootstrap.min.css
            │   │       ├── 📄 clean-blog.min.css
            │   │       └── 📄 .LCKbootstrap.min.css~
            │   │
            │   ├── 📂 fonts
            │   │   ├── 📄 font-awesome.css
            │   │   ├── 📄 fontawesome-webfont.eot
            │   │   ├── 📄 fontawesome-webfont.svg
            │   │   ├── 📄 fontawesome-webfont.ttf
            │   │   ├── 📄 fontawesome-webfont.woff
            │   │   ├── 📄 fontawesome-webfont.woff2
            │   │   └── 📄 FontAwesome.otf
            │   │
            │   ├── 📂 images
            │   │   ├── 📄 404.png
            │   │   ├── 📄 505.png
            │   │   ├── 📄 favicon.png
            │   │   └── 📄 intro.jpg
            │   │
            │   └── 📂 js
            │       ├── 📄 app.js
            │       │
            │       ├── 📂 scripts
            │       │   ├── 📂 configs
            │       │   │   └── 📄 tablepost.js
            │       │   │
            │       │   ├── 📂 controllers
            │       │   │   ├── 📄 LoginController.js
            │       │   │   └── 📄 PostController.js
            │       │   │
            │       │   ├── 📂 functions
            │       │   │   └── 📄 alert.js
            │       │   │
            │       │   └── 📂 services
            │       │       └── 📄 services.js
            │       │
            │       └── 📂 vendor
            │           ├── 📄 angular.min.js
            │           ├── 📄 angular-datatables.min.js
            │           ├── 📄 bootstrap.bundle.min.js
            │           ├── 📄 clean-blog.min.js
            │           ├── 📄 jquery.min.js
            │           ├── 📄 jquery.dataTables.min.js
            │           ├── 📄 ng-file-upload.js
            │           └── 📄 ng-file-upload-shim.js
            │
            └── 📂 WEB-INF
                ├── 📄 applicationContext.xml
                ├── 📄 dispatcher-servlet.xml
                ├── 📄 web.xml
                │
                ├── 📂 jsp
                │   ├── 📂 errors
                │   │   ├── 📄 404.jsp
                │   │   └── 📄 505.jsp
                │   │
                │   ├── 📂 post
                │   │   ├── 📄 edit.jsp
                │   │   ├── 📄 index.jsp
                │   │   ├── 📄 new.jsp
                │   │   └── 📄 show.jsp
                │   │
                │   └── 📂 usersys
                │       └── 📄 login.jsp
                │
                └── 📂 tags
                    ├── 📄 _layout.tag
                    └── 📄 .LCK_layout.tag~
