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
11. Interfaces with the HR department legacy systems to retrieve required employee information and changes

# Non-Functional Requirements

1. The system must be easy to use
2. Save time and money mostly in the HR department
3. Improve the internal business processes of this organization, at least with respect to the time it takes to manage vacation time requests

## Constraints

1. Web Application
2. The VTS must use the Central Authentication Service (CAS) for user identification, as it is an extension of the existing company intranet portal
3. The application must function properly on all HTML 3.2–capable browsers
4. The architecture must account for the fact that the client and server are only connected long enough to process a single request, requiring a robust client state management mechanism (such as cookies or URL redirection)

## Manage Time Use Case Diagrams

### Entity Relationship Diagram

![VTS ERD](use-cases/manage-time/erd/vts-erd.png)

### Flowcharts

![Create New Request](use-cases/manage-time/flowcharts/create-new-request.png)

Create New Request

![Edit Request](use-cases/manage-time/flowcharts/edit-request.png)
Edit Request

![Withdraw Request](use-cases/manage-time/flowcharts/withdraw-request.png)

Withdraw Pending Request

![Cancel Approved Request](use-cases/manage-time/flowcharts/cancel-approved-request.png)
Cancel Approved Request
