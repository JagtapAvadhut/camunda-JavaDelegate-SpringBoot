# Camunda Workflow with Spring Boot

This project demonstrates how to integrate **Camunda** workflow engine with **Spring Boot**, featuring a simple leave
approval process.

## Features

- Camunda BPM engine integration with Spring Boot
- Leave approval workflow
- User tasks and service tasks
- Process modeling using BPMN
- Notification service
- In-memory H2 database for persistence

## Prerequisites

Before you begin, ensure you have the following installed:

- **Java 17** or above
- **Maven** 3.6 or above
- **Camunda Modeler** (optional for BPMN modeling)
- **Git**

## Technologies Used

- **Spring Boot 3.2.2**
- **Camunda BPM 7.21.0**
- **H2 Database**
- **Java 17**

## Dependencies

This project includes the following dependencies:

- `org.camunda.bpm.springboot:camunda-bpm-spring-boot-starter-rest`
- `org.camunda.bpm.springboot:camunda-bpm-spring-boot-starter-webapp`
- `org.camunda.bpm:camunda-engine-plugin-spin`
- `org.camunda.spin:camunda-spin-dataformat-all`
- `com.h2database:h2`

## Project Structure

The structure of the project is as follows:

## Step-by-Step Instructions

### Step 1: Clone the Repository

First, clone the project repository to your local machine:

### Step 2: Build the Project

### Step 3: Run the Application

### Step 4: Access Camunda Web Interface

http://localhost:8080

Login with the default credentials:
Username: demo
Password: demo

### Step 5:  Login with the default credentials:

Username: demo
Password: demo

### Step 6: Process Explanation

Start Event: The process starts when a leave request is initiated.
LeaveApproval Service Task: This service task executes the LeaveApproval class.
Manager User Task: The manager reviews the leave request.
HR User Task: The HR team finalizes the approval.
Notification Service Task: Sends a notification after approval using the Notification class.
End Event: Marks the end of the workflow.

### Step 7: Testing the Workflow

To test the workflow:

Navigate to the Camunda Tasklist on the web interface.
Start a new process instance for the leave approval process.
Complete the user tasks (Manager and HR approval) as assigned.

### Step 8: Customization

You can customize the process by modifying the BPMN file or adding new Java delegate classes to handle additional logic.

### Author

Avadhut Jagtap 

```bash
git clone https://github.com/JagtapAvadhut/camunda-with-Spring-Boot.git
cd camunda-with-Spring-Boot

mvn clean install
mvn spring-boot:run

http://localhost:8080

