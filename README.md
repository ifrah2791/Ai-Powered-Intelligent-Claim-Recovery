# AI-Powered Intelligent Claim Recovery Workflow

## Overview

AI-Powered Intelligent Claim Recovery Workflow is an end-to-end
intelligent automation solution built using UiPath Agent Builder,
Maestro BPMN, UiPath Apps, RPA, MCP Servers, and AI Agents to automate
healthcare claim recovery.

## Problem Statement

Healthcare claim recovery is manual, time-consuming, error-prone, and
difficult to audit. Teams spend significant effort identifying payment
variances, root causes, and recovery actions.

## Solution

The solution orchestrates AI agents and UiPath automation to screen
claims, detect overpayments/underpayments, investigate root causes,
recommend recovery actions, and route high-risk cases for human
approval.

## Workflow

1.  Claim Retrieval
2.  Screening Agent
3.  Detection & Validation Agent
4.  Root Cause Investigation Agent
5.  Human Validation
6.  Recovery Decision

## AI Agents

### Claim Recovery Screening Agent

-   Input: Claim ID
-   Output: High Risk (Yes/No)

### Detection & Validation Agent

Outputs: - Recovery Type - Expected Amount - Paid Amount - Variance
Amount

### Root Cause Investigation Agent

Outputs: - Root Cause - Confidence Score - AI Recommendation - Suggested
Recovery Actions

## High-Risk Conditions

-   Paid Amount \> \$100
-   Duplicate Payment
-   COB Review Required
-   Missing Modifier
-   Large Payment Variance
-   High Billed Amount
-   Senior Member
-   Paid Claim Status

## UiPath Components

-   Maestro BPMN
-   Agent Builder
-   UiPath Apps
-   MCP Server
-   Orchestrator
-   Action Center
-   RPA
-   AI Center

## MCP Tools

-   ClaimRecoveryDetails
-   ClaimDOSDetails

## Benefits

-   Faster investigations
-   Explainable AI
-   Human-in-the-loop governance
-   Complete audit trail
-   Reduced manual effort
-   Scalable architecture

## Technology Stack

-   UiPath Platform
-   FastAPI
-   Python
-   HTML/CSS/JavaScript
-   REST APIs
-   GitHub

## Future Enhancements

-   Predictive recovery prioritization
-   Automated appeals
-   Analytics dashboard
-   Continuous learning

## Team

**Firstsource Neural Squad**

Project: **AI-Powered Intelligent Claim Recovery Workflow**

## License

Apache 2.0 License

## Acknowledgements

Built for the UiPath Hackathon to demonstrate intelligent healthcare
claim recovery using AI Agents and UiPath Automation.
