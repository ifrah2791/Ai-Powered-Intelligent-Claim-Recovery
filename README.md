# AI-Powered Intelligent Claim Recovery Workflow

## Overview

AI-Powered Intelligent Claim Recovery Workflow is an end-to-end healthcare claims recovery solution built using the UiPath Business Automation Platform. The solution leverages Low-Code AI Agents, UiPath Maestro BPMN, UiPath Apps, MCP Server, Data Fabric, RPA, and Human-in-the-Loop validation to intelligently identify payment variances, determine root causes, and recommend recovery actions.

The solution automates the complete claim recovery lifecycle—from claim retrieval and AI-based risk screening through payment validation, root-cause investigation, and human approval—providing a scalable, explainable, and auditable recovery process.

---

# Agent Type

This solution uses **Low-Code Agents only**.

No coded agents were used in this project.

The following Low-Code Agents were built using **UiPath Agent Builder**:

* Claim Recovery Screening Agent
* Detection & Validation Agent
* Root Cause Investigation Agent

---

# Solution Architecture

```
Local Claims Application
            │
            ▼
      FastAPI Service
            │
            ▼
       UiPath Apps
            │
            ▼
     Maestro BPMN Process
            │
            ▼
 Claim Recovery Screening Agent
            │
            ▼
 Detection & Validation Agent
            │
            ▼
 Root Cause Investigation Agent
            │
            ▼
      UiPath Action Center
            │
            ▼
      Human Approval
```

---

# Technologies Used

## UiPath

* UiPath Maestro BPMN
* UiPath Agent Builder
* UiPath Apps
* UiPath Orchestrator
* UiPath MCP Server
* UiPath Data Fabric
* UiPath Action Center

## Backend

* FastAPI
* Python
* REST APIs
*Node js

## Frontend

* HTML
* CSS
* JavaScript

---

# AI Agents

## 1. Claim Recovery Screening Agent

Purpose

* Retrieves claim details
* Evaluates High-Risk conditions
* Routes only eligible claims for investigation

Output

* High Risk (Yes/No)

---

## 2. Detection & Validation Agent

Purpose

* Calculates expected reimbursement
* Compares paid amount
* Determines payment variance

Output

* Recovery Type
* Expected Amount
* Paid Amount
* Variance Amount

---

## 3. Root Cause Investigation Agent

Purpose

Determines the most probable reason for payment variance and recommends recovery actions.

Output

* Root Cause
* Confidence Score
* AI Recommendation
* Suggested Recovery Actions

---

# MCP Server Tools

## ClaimRecoveryDetails

Retrieves:

* Claim Details
* Member Details
* Provider Details
* Payment Information

## ClaimDOSDetails

Retrieves:

* Date of Service
* Diagnosis Code
* Diagnosis Description
* Provider Details

---

# Project Structure

```
Claim-Recovery/
│
├── ClaimRecoveryAPI/
│      FastAPI Project
│
├── ClaimRecoveryApp/
│      Local Web Application
│
├── DummyData/
│      Claims Dataset
│      
│      
│
├── UiPath/
│      BPMN Process
│      Agents
│
└── README.md
```

---

# Prerequisites

Before running the solution, ensure the following software is installed:

* Python 3.11 or later
* Git
* UiPath Studio
* UiPath Orchestrator
* UiPath Apps
* UiPath Agent Builder
* UiPath Data Fabric
* Modern Web Browser
* Node.js

---

# Setup Instructions

## Step 1 – Download Repository

Clone or download the GitHub repository.

```
git clone <Repository URL>
```

or

Download the ZIP file and extract it.

---

## Step 2 – Start the FastAPI Service

Open Command Prompt.

Navigate to the API folder.

Example

```
cd ClaimRecoveryAPI
```

Install dependencies.

```
npm install express

```

Run the API.

```
node server.js
```

The API will start locally.

Example:

```
http://localhost:4000
```

---

## Step 3 – Start the Local Claims Application

Open another Command Prompt.

Navigate to the Claims Application folder.

Example

```
cd ClaimRecoveryApp
```

Start the application.

Example

```
npm install
npm start
```

(or execute the appropriate startup command included in this repository.)

Open

```
http://localhost:3000/login.html
```

in your chrome browser.

---

## Step 4 – Configure UiPath Data Fabric

Create a new Data Fabric entity using the same entity names included in this repository.

Import the provided sample datasets from the **DummyData** folder.

Required entities include:

* Claims


The sample CSV files included in the repository can be imported directly.

---

## Step 5 – Configure MCP Server

Create the MCP Server in UiPath Orchestrator.

Server Name

```
claim-recovery-process-mcp-01
```

Add the following tools:

* ClaimRecoveryDetails
* ClaimDOSDetails

---

## Step 6 – Import UiPath Components

Import:

* Maestro BPMN Process
* AI Agents
* UiPath App

Configure all connections as described in the project documentation.

---

## Step 7 – Execute the Demo

1. Launch the Local Claims Application.
2. Search using a sample Claim ID.
3. Submit the claim.
4. The Screening Agent evaluates risk.
5. Detection & Validation Agent calculates payment variance.
6. Root Cause Investigation Agent determines the recovery reason.
7. High-risk claims are routed to Action Center for approval.

---

# Sample Data

The repository contains sample datasets for demonstration.

These datasets include:

* Claims


Use these files to populate UiPath Data Fabric.

---

# Human-in-the-Loop

High-risk claims are automatically routed to UiPath Action Center where reviewers can:

* Approve Recovery
* Reject Recovery
* Escalate to SME

Every action is fully auditable.

---

# Benefits

* Automated Claim Screening
* AI-Powered Payment Validation
* Intelligent Root Cause Detection
* Human-in-the-Loop Governance
* Explainable AI Decisions
* Complete Audit Trail
* Reduced Manual Investigation
* Faster Recovery Processing

---

# Team

**Firstsource Neural Squad**

Project:

**AI-Powered Intelligent Claim Recovery Workflow**

---

# License

Appace 2.0

---

# Acknowledgements

Built for the UiPath Hackathon using UiPath Agent Builder, Maestro BPMN, UiPath Apps, MCP Server, Data Fabric, and Human-in-the-Loop automation to demonstrate an enterprise-ready AI-powered healthcare claim recovery solution.
