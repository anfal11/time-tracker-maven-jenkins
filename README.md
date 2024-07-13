# time-tracker
Java (Maven) application for tracking time on the job

Time tracker

# Building a Maven Project with Jenkins on Windows

This guide provides a detailed walkthrough for setting up and building a Maven project using Jenkins on a Windows machine.

## Prerequisites

- **Windows OS**
- **Jenkins** installed
- **Maven** installed
- **Git** installed (optional but recommended)

## Step-by-Step Instructions

### 1. Install Jenkins

- Download the Jenkins installer for Windows from the [official Jenkins website](https://www.jenkins.io/download/).
- Run the installer and follow the on-screen instructions to complete the installation.
- Once installed, start Jenkins.

### 2. Install Maven

- Download the Maven binary zip archive from the [Apache Maven website](https://maven.apache.org/download.cgi).
- Extract the contents to a suitable directory, e.g., `C:\Program Files\Apache\Maven`.
- Set the `MAVEN_HOME` environment variable to the Maven directory.
- Add the Maven `bin` directory to the `PATH` environment variable.

### 3. Configure Jenkins for Maven

- Navigate to the Jenkins Dashboard and go to `Manage Jenkins > Global Tool Configuration`.
- Scroll to the "Maven" section and click `Add Maven`.
- Provide a name (e.g., `Maven`) and set the `MAVEN_HOME` to your Maven installation directory.

### 4. Create a Jenkins Job for Your Maven Project

- On the Jenkins Dashboard, click `New Item`.
- Enter a name for your job, select `Freestyle project`, and click `OK`.
- In the job configuration page:
  - Under `Source Code Management`, select `Git` and provide your repository URL (if applicable).
  - Under `Build`, click `Add build step` and select `Invoke top-level Maven targets`.
  - In the `Goals` field, enter `clean install` (or other Maven goals as needed).

### 5. Build the Project

- Save the job configuration.
- Click `Build Now` to start the build process.
- Monitor the build progress in the `Console Output`.

## Benefits

- **Automation:** Streamline your build process with Jenkins.
- **Integration:** Easily integrate with various tools and services.
- **Efficiency:** Improve project management and deployment speed.

---

Happy coding! 🎉

---

This guide aims to be straightforward and helpful for anyone looking to set up Jenkins with Maven on Windows. Let me know if you need any additional information or assistance!
