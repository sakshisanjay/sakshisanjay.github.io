---
title: Setting up a Test Project in Selenium using .NET C#
layout: blog
category: [Selenium, Automation]
excerpt: In this blog, I will share the steps of how to setup a simple project to be automation tested with Selenium in .NET with C# programming language.
comments: true
---

In this blog, I will share the steps of how to setup a simple project to be automation tested with Selenium in .NET with C# programming language. Here, I assume that you are completely new to Selenium and your machine needs to be configured from scratch.

Here, we will focus on doing automation test with Chrome browser using Selenium.

### STEP 1. Download and Install Visual Studio

Download [Visual Studio Community Edition](https://visualstudio.microsoft.com/)

![VS](https://sakshimehta.s3-ap-southeast-1.amazonaws.com/images/vs.png)

The installation of Visual Studio Community Edition is pretty straight forward. Just double click the installer and install.

> Ensure to select the "ASP.NET and web development" workload in the installation wizard

![ASP NET Workload](https://sakshimehta.s3-ap-southeast-1.amazonaws.com/images/asp-net-workload.png)

### STEP 2. Chrome Browser

1. Download and Install [Chrome Browser](https://www.google.com/chrome/) (if not already installed)
2. Update the [Chrome Browser to latest version](https://www.wikihow.com/Update-Google-Chrome)

### STEP 3. Download and Configure Chrome Driver

1. Download the latest **stable release** of [Chrome Driver](https://chromedriver.chromium.org/downloads).
1. Unzip the downloaded zip file
1. Put the chromedriver.exe from the unzip folder to a new folder named "Drivers" (ideally in C or D Drive)
1. Copy the path of the "Drivers" folder
1. Click the Windows button & Open "View Advanced System Settings"
1. Click on "Environment Variables" button
1. Select the "Path" under System Variables and click on Edit
1. Click on New button
1. Paste the copied "Drivers" folder location
1. Click OK
1. Close the Environment Variables window

What we did so far ensures that the driver is registered in the system variables path. This will make sure that the selenium code is able to call the driver.

We can test if the driver is registered properly by following the steps below:

- Open "Command prompt"
- Type the command "chromedriver" and press enter

You should see a message that states the ChromeDriver is starting. Optionally, press Ctrl+C in command prompt to stop the chrome driver that we started.
![Chrome Driver Running](https://sakshimehta.s3-ap-southeast-1.amazonaws.com/images/chromedriver-success.PNG)

### STEP 4. Install AutoIT

1. Download the [AutoIT software](https://www.autoitscript.com/site/autoit/downloads/)
   ![AutoIT](https://sakshimehta.s3-ap-southeast-1.amazonaws.com/images/autoit.png)
2. Double click the downloaded .exe file and install

### STEP 5. Preparing Visual Studio with Automation tools

1. Launch Visual Studio and click on "Continue without code"
   ![VS Without Code](https://sakshimehta.s3-ap-southeast-1.amazonaws.com/images/vs-without-code.png)
2. Click on "Manage Extension" option under the "Extensions" Tab in Visual Studio
3. Click on "Online" Tab
4. Search for "NUnit Test Adapter" and download the extension
5. Close the Visual Studio so that the downloaded extension starts installing
6. Click on the "Modify" button when the extension installation automatically starts
7. Once finished, click on "Close" button

Now, we have completed all the steps required to make our environment ready for Automation Testing using Selenium.

### Creating a Test Project

1. Open Visual Studio again
2. Click "Create a new project" button and select "Console Application C#"
3.
