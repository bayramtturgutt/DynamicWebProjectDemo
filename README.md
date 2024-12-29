# Dynamic Web Project Setup Guide

This guide will walk you through setting up and running the Dynamic Web Project using Apache Tomcat on Eclipse IDE.

---

## Prerequisites

Before you start, ensure you have the following installed on your system:

1. **Java Development Kit (JDK)**
   - [Download JDK](https://www.oracle.com/java/technologies/javase-downloads.html)

2. **Eclipse IDE for Java EE Developers**
   - [Download Eclipse IDE](https://www.eclipse.org/downloads/)

3. **Apache Tomcat Server**
   - [Download Tomcat 10.1.19](https://tomcat.apache.org/download-10.cgi)

---

## Steps to Start the Project

### 1. Import Project into Eclipse

1. Open Eclipse IDE.
2. Go to `File > Import`.
3. Select `Existing Projects into Workspace` and click `Next`.
4. Browse to the folder containing the Dynamic Web Project files and click `Finish`.

### 2. Configure Apache Tomcat Server in Eclipse

1. Go to `Window > Preferences`.
2. Navigate to `Server > Runtime Environments`.
3. Click `Add`.
4. Select `Apache > Tomcat v10.0` and click `Next`.
5. Browse to the location where you extracted the Apache Tomcat server and click `Finish`.
6. Click `OK` to close the Preferences window.

### 3. Add Tomcat Server to the Project

1. Open the `Servers` tab at the bottom of Eclipse.
   - If the `Servers` tab is not visible, go to `Window > Show View > Servers`.
2. Right-click in the `Servers` tab and select `New > Server`.
3. Choose `Apache > Tomcat v10.0` and click `Next`.
4. Select the installed Tomcat runtime and click `Next`.
5. Add your Dynamic Web Project to the `Configured` list and click `Finish`.

### 4. Run the Project on Tomcat Server

1. Right-click on the newly added Tomcat server in the `Servers` tab.
2. Select `Start` to start the server.
3. Once the server is running, right-click on your project in the `Project Explorer`.
4. Select `Run As > Run on Server`.
5. Choose the configured Tomcat server and click `Finish`.
6. Your project will be deployed, and the default web browser will open with the project’s homepage.

---

## Testing the Project

1. Navigate to the examples listed on the homepage (`index.html`).
2. Interact with the features such as forms, AJAX examples, or API integrations.

---

## Troubleshooting

- **Error: Tomcat not starting**
  - Ensure the port (default is 8080) is not in use by another application.
  - Check if the correct JDK version is configured in Eclipse.

- **Project not deploying correctly**
  - Clean the project by going to `Project > Clean` and redeploying.
  - Verify that all project dependencies are correctly configured.

---

## Additional Resources

- [Eclipse Documentation](https://help.eclipse.org/)
- [Apache Tomcat Documentation](https://tomcat.apache.org/tomcat-10.0-doc/)
- [Java Tutorials](https://docs.oracle.com/javase/tutorial/)
