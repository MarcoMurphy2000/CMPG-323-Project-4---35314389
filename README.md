# CMPG-323-Project-4---35314389
# Testing and RPA <br />

## Background <br />
Acceptance testing also known as user acceptance testing (UAT) is a crucial part in the development of any solution. The goal is to ensure that the input produces the expected outcome over a series of predefined test runs. This is to account for the potential event of a runtime error or any other reason for the test failing for a reason not related to the solution. The solution would typically not be released untill it passes all the tests in UAT. <br />
Testing can be a laborous, repetitive, and time consuming process. Ideally, instead of testing a solution, developers or workers can spend their time on immersive tasks. Robotic process automation (RPA) is the solution the this issue. It is software technology that makes it easy to build, deploy, and manage software robots that imitate the ineraction between software solutions and humans. Software robots can do things like understand what’s on a screen, complete the right keystrokes, navigate systems, identify and extract data, and perform a wide range of defined actions. But software robots can do it faster and more consistently which can save a comapny time while having their employees focus on different perhaps more creative jobs. <br />
For the web application created in Project 3, before this solution could be published, it would have to pass (UAT). This task would usually be performed by a team of "testers" entrusted dataset for input to test weather or not the desired output will be produced. Project 4 requires the creation of a software robot to do this task of testing the solution. <br /><br />

## How to use the project (for users)
The project consists of a "create" workflow and a "read, update & delete" workflow. ><br />
The create workflow once excecuted will try to create each row in the provided excel workbook sheet. Simply put, there are 3 main sequences for the create workflow. Each sequence takes one of the sheets in the workbook (Zone, Category, Device) and places that specific sheets data in a dataTable which it the used to insert the row data into the web appplication. AFter each row has been inserted, the value is looked for to ensure that it has been created. If so, the ecel wrkbook test results sheet is updated at that values specific cell (TRUE or false). This logic is used throughout the project for read, update and delete. <br />
The "read, update & delete" workflow checks if the value can be read and the updates the excel worksheet. Checks if it can be edited. Updated the excel worksheet. And finally tries to delete a row value, followed by an update to the excel worksheet. This process is followed for each sheet (Zone, Category, Device).<br /><br />

## Project published to uipath orchestrator service <br />
![image](https://user-images.githubusercontent.com/53267265/198121502-181403a2-f1ea-44b3-bf03-4d5beba87317.png)

