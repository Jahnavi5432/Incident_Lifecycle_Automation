# Incident Lifecycle Automation in ServiceNow

## Project Overview

This project demonstrates the implementation of an Incident Lifecycle Automation process in ServiceNow. The project covers incident creation, classification, assignment, knowledge integration, escalation, resolution, and validation.

## Project Objectives

- Create and manage incidents in ServiceNow
- Classify incidents based on category and priority
- Assign incidents to appropriate assignment groups
- Track incident status throughout its lifecycle
- Integrate knowledge articles with incidents
- Manage parent and child incidents
- Handle emergency change requests
- Resolve incidents and document the resolution
- Validate related records and SLA information

## ServiceNow Implementation

### 1. Service Creation

A **Remote Access** service was created to support the incident management process.

### 2. Service Offering

A **Corporate VPN** service offering was created under the Remote Access service.

### 3. Incident Creation

Incidents were created for VPN-related issues.

Example:

- **Incident:** INC0010001
- **Short Description:** Unable to connect to Corporate VPN from home office
- **Category:** Network
- **Subcategory:** VPN
- **Service:** Remote Access
- **Service Offering:** Corporate VPN
- **State:** Resolved

The incident report also contains assignment, work notes, comments, related configuration items, and SLA information.

### 4. Incident Classification and Assignment

The incident was classified and assigned to the appropriate support group for further processing.

### 5. Knowledge Integration

Knowledge articles were applied to incidents to support troubleshooting and resolution.

Example:

- **KB0010001:** Unable to connect to Corporate VPN from home office
- **KB0005012:** What to do when you are locked out of your computer?

### 6. Parent and Child Incident

A child incident was associated with the parent incident.

Example:

- **Parent Incident:** INC0010001
- **Child Incident:** INC0010005

INC0010005 was resolved based on the resolution of its parent incident.

### 7. Incident Resolution

The probable cause was identified as a suspended PowerEdge service.

The resolution involved restarting the VPN-SRV-02 service as part of an emergency change request.

### 8. Knowledge Creation

A knowledge article was created for the VPN issue:

- **Knowledge Article:** KB0010002
- **Title:** Unable to connect to Corporate VPN

## Tools and Technologies

- ServiceNow
- Service Operations Workspace
- Incident Management
- ITSM
- Knowledge Management
- Configuration Management Database (CMDB)
- Service Level Agreements (SLA)
- Update Sets

## Project Evidence

The `reports` folder contains the ServiceNow incident reports used as project evidence.

### Reports
- `Incident-INC0010001-Report.pdf`
- `Incident-INC0010005-Report.pdf`


These reports demonstrate incident details, resolution information, related records, SLA information, configuration items, and knowledge integration.

## Project Structure

```text
Incident-Lifecycle-Automation-ServiceNow/
│
├── README.md
├── reports/
│   ├── Incident-INC0010001-Report.pdf
│   └── Incident-INC0010005-Report.pdf
│
└── screenshots/
    ├── service-created.png
    ├── service-offering.png
    ├── incident-created.png
    ├── incident-classification.png
    ├── incident-resolution.png
    └── knowledge-article.png

## Conclusion

The project demonstrates the Incident Lifecycle in ServiceNow, from incident creation and classification through assignment, knowledge integration, related record management, and final resolution.
