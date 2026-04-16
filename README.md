# Vision

A Vacation Tracking System (VTS) will provide individual employees with the capability to manage their own vacation time, sick leave, and personal time off, without having to be an expert in company policy or the local facility’s leave
policies.

# Functional Requirements

1. Implements a flexible rules-based system for validating and verifying leave time requests
2. Enables manager approval (optional)
3. Provides access to requests for the previous calendar year, and allows requests to be made up to a year and a half in the future
4. Uses e-mail notification to request manager approval and notify employees of request status changes
5. Uses existing hardware and middleware
6. Is implemented as an extension to the existing intranet portal system, and uses the portal’s single-sign-on mechanisms for all authentication
7. Keeps activity logs for all transactions
8. Enables the HR and system administration personnel to override all actions restricted by rules, with logging of those overrides
9. Allows managers to directly award personal leave time (with system-set limits)
10. Provides a Web service interface for other internal systems to query any given employee’s vacation request summary
11. Integrate with the HR department legacy systems to retrieve required employee information and changes

# Non-Functional Requirements

1. The system must be easy to use(reusable)
2. Save time and money mostly in the HR department
3. Improve the internal business processes of this organization, at least with respect to the time it takes to manage vacation time requests

## Constraints

1. Integration: Integrate with HR department legacy systems to retrieve employee information and changes
2. Single-Sign-On (SSO): The VTS must use the Central Authentication Service (CAS) for user identification, as it is an extension of the existing company intranet portal
3. Hardware: Uses existing hardware
4. Integration as an Intranet Extension : The VTS is explicitly defined as an extension of the existing company intranet portal
   . By building it as a Web-centric application integrated into the current infrastructure, the system provides a natural entry point for users who are already familiar with the company's internal tools

## Actors

- Employee
- Manager
- HR
- Admin

## Tools Used for Diagrams

- [dbdiagram.io](https://dbdiagram.io/)
- [Lucid](https://lucid.app/)
- [Mermaid](https://mermaid.ai/)

## Manage Time Use Case Diagrams

### Entity Relationship Diagram

[![VTS ERD](use-cases/manage-time/erd/vts-erd.png)](https://dbdiagram.io/d/69da41f18089629684718610)

[View Live ERD on dbdiagram.io](https://dbdiagram.io/d/69da41f18089629684718610)

[Open ERD image](use-cases/manage-time/erd/vts-erd.png)

### Flowcharts

![Create New Request - Employee](use-cases/manage-time/flowcharts/create-new-request-employee.png)

[Open image](use-cases/manage-time/flowcharts/create-new-request-employee.png)

Create New Request (Employee)

![Create New Request - Manager](use-cases/manage-time/flowcharts/create-new-request.png)

[Open image](use-cases/manage-time/flowcharts/create-new-request.png)

Create New Request (Manager)

![Edit Request](use-cases/manage-time/flowcharts/edit-request.png)

[Open image](use-cases/manage-time/flowcharts/edit-request.png)

Edit Request

![Withdraw Request](use-cases/manage-time/flowcharts/withdraw-request.png)

[Open image](use-cases/manage-time/flowcharts/withdraw-request.png)

Withdraw Pending Request

![Cancel Request](use-cases/manage-time/flowcharts/cancel-request.png)

[Open image](use-cases/manage-time/flowcharts/cancel-request.png)

Cancel Request

### Sequence Diagrams

![Create New Request - Employee](use-cases/manage-time/sequence-diagrams/create-new-request-employee.png)

[Open image](use-cases/manage-time/sequence-diagrams/create-new-request-employee.png)

Create New Request (Employee)

![Create New Request - Manager](use-cases/manage-time/sequence-diagrams/create-request-manager.png)

[Open image](use-cases/manage-time/sequence-diagrams/create-request-manager.png)

Create New Request (Manager)

![Edit Request](use-cases/manage-time/sequence-diagrams/edit-request.png)

[Open image](use-cases/manage-time/sequence-diagrams/edit-request.png)

Edit Request

![Withdraw Request](use-cases/manage-time/sequence-diagrams/withdraw-request.png)

[Open image](use-cases/manage-time/sequence-diagrams/withdraw-request.png)

Withdraw Pending Request

![Cancel Request](use-cases/manage-time/sequence-diagrams/cancell-request.png)

[Open image](use-cases/manage-time/sequence-diagrams/cancell-request.png)

Cancel Request

### Pseudocode

[Employee pseudocode](use-cases/manage-time/pseudocode/employee-pseudocode.txt)

[Manager pseudocode](use-cases/manage-time/pseudocode/manager-pseudocode.txt)

### UI

![Vacation Requests UI](use-cases/manage-time/ui/list-vacation-requests.png)

[Open UI image](use-cases/manage-time/ui/list-vacation-requests.png)

## HR Approval Challenge

### Pseudocode

[Employee pseudocode](use-cases/challenges/hr-approval/pseudocode/employee--pseudocode.txt)

[Manager pseudocode](use-cases/challenges/hr-approval/pseudocode/manager--pseudocode.txt)

[HR pseudocode](use-cases/challenges/hr-approval/pseudocode/hr-pseudocode.txt)

### ERD

![HR Approval ERD](use-cases/challenges/hr-approval/erd/hr-approval.png)

[Open ERD image](use-cases/challenges/hr-approval/erd/hr-approval.png)

![Workflow Status ERD](use-cases/challenges/hr-approval/erd/workflow-status.png)

[Open workflow status image](use-cases/challenges/hr-approval/erd/workflow-status.png)

### Sequence Diagram

![HR Approval Sequence Diagram](use-cases/challenges/hr-approval/sequence-diagram/hr-approval.png)

[Open sequence diagram image](use-cases/challenges/hr-approval/sequence-diagram/hr-approval.png)

### State Machine Diagram

![HR Approval State Machine Diagram](use-cases/challenges/hr-approval/state-machine-diagram/Screenshot%20from%202026-04-17%2001-02-36.png)

[Open state machine diagram image](use-cases/challenges/hr-approval/state-machine-diagram/Screenshot%20from%202026-04-17%2001-02-36.png)
