# Simple Java Maven Build with Jenkins

## Overview

This project is a basic Java application set up with Maven and built using Jenkins for Continuous Integration (CI).  
You will learn how to build, test, and automate a Java application using free, open-source tools.

---

## Folder Structure

simple-java-app/
├── pom.xml
├── README.md
└── src/
    ├── main/
    │   └── java/
    │       └── com/
    │           └── example/
    │               └── App.java
    └── test/
        └── java/
            └── com/
                └── example/
                    └── AppTest.java


---

## How to Build Locally

- mvn clean install

`This will produce a file like `target/simple-java-app-1.0-SNAPSHOT.jar`

---

## How to Build in Jenkins

1. **Create a New Freestyle Project**
    - Source Code Management: Git → use your repo’s URL.
    - Build Step: Add “Invoke top-level Maven targets” with the goal `clean install`.
    
2. **Run the Build**
    - Click **Build Now** in Jenkins.
    - Check Console Output for build and test status.

---

## Screenshots

### Jenkins build success output

- Jenkins job configuration and build success:
  - ![Jenkins Build Success](images/jenkins-success-console.png)
    
---

  - ![Jenkins Success Build Output](images/jenkins-success-console-1.png)

---

### JAR file in Target

- JAR file present in `target/` folder:
  - ![JAR File in Target](images/jar-in-target-folder.png)

---

## Author

- S NAGAVEENA

