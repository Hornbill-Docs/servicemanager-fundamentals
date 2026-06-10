# Incident Management

Incident management is a critical process in IT service management (ITSM) that focuses on restoring normal service operation as quickly as possible following an incident, while minimizing the impact on business operations. An incident is defined as an unplanned interruption to an IT service or a reduction in the quality of an IT service. The goal of incident management is to ensure that incidents are resolved efficiently and effectively, while also providing a positive experience for users.

## Incident Record Creation

### Incident Record Creation Methods

Incident records can be created by various methods; this must include, at a minimum:

- A manual entry
- From an email
- Submitted by a user via the portal/service catalog with user-entered fields that populate the incident record
- Launched through a monitored alert notification
- From a chat session (manual chat or chatbot); all interaction/communication should be included in the incident record
- Launched from a service request record
- Launched from a change record

---

### Incident Templates

Client admins can create and apply templates for different types of incidents with different forms, fields, and possibly prefilled data depending on the type of incident. Examples of incident types can include standard/simple incidents, complicated incidents, major incidents, security incidents, and incidents for specific services or customer departments — and are client definable.

---

### Incident Models

Client admins can create and apply specific incident models for different types of incidents; models include templates (see IM2) and different workflows specific to the type of incident.

---

### Chat Session Integration

Incident records can be created and updated through a chat session with information from the chat session input into the incident record, and the necessary effort needed to manually update the record is reduced or eliminated. Where chatbots are utilized: an incident record can be systematically created with chat session information without the need for any human interaction to complete the incident record, including the proper categorization.

---

### Duplicate Incident Detection

Identify duplicate incidents and flag these incidents for appropriate action to be taken by the client.

---

## Categorization & Classification

### Service, Component, and Asset Linking

Multiple service, component, and asset records can be searched for in the respective repositories, from within the incident record, and applied or linked to the incident. These records can be distinguished as to whether they are the cause of the incident or impacted or affected by the incident.

---

### Category Structure

Clients can define an incident category structure that is unique to their organization. The category structure can include a related or dynamic tiered level of categories, as well as include the selected service, component, and IT asset records.

---

### Category-Triggered Actions

The defined category structure (refer to IM7) can be used to inform or trigger the following actions, at a minimum:

- Identify and apply the assignment group/technician
- Perform a trend analysis to identify and use information from related incidents, problems, and changes
- Search for and utilize related knowledge articles

---

## Prioritization & First-Call Resolution

### Incident Prioritization

A method to prioritize incidents is available that can be based on risk, lead time, level of effort, severity, business need, workload, and other client-defined criteria.

---

### First-Call Resolution

First-call resolution (first contact resolution, etc.) can be defined by the client, measured, and reported independently from the defined prioritization method.

---

## Diagnosis & Resolution

### Problem Record Integration

Problems can be searched for, from within any incident record, and workaround or resolution information found in these records can be systematically applied to the incident record. The problem record can be linked with or related to the incident record.

---

### Knowledge Article Integration

Knowledge articles can be searched for, from within any incident record, and information contained in the article can be systematically applied to the incident record. Additionally, the knowledge articles can be linked to the incident.

---

### Remote Diagnostic Support

Remote diagnostic support tools can be used, and triggered from within the incident record, and the remote session logs can be saved in or linked to the incident record.

---

### Detailed Diagnosis and Resolution

Detailed diagnosis and resolution information can be recorded in the incident record, as well as identify the following information. This must include, at a minimum:

- Statuses throughout the life cycle of the incident to be either systematically set based on the incident model or workflow, or can be manually entered
- A resolution or closure category or reason code, that can be tracked and reported separately from the initial category that was selected when the incident was initially logged
- Identification of a service component that may be causing the incident, which may be different from the initial component that was identified
- The ability to identify non-technical causes or contributors to the incident
- Resolution type (for example, resolved, applied known workaround, unresolved/unknown, etc.)

---

## Major Incidents

### Major Incident Identification

A major incident record can be identified and can be distinguished from other types of incidents with unique templates, models, workflows, prioritization, and notifications. Multiple non-major incidents may be linked to a single major incident record.

---

### Major Incident Creation & Promotion

Major incidents can be manually created, promoted (or updated) from a non-major incident, or can be systematically launched by pre-defined criteria. Clients should be able to define these criteria for their organization, though some capability may be provided out-of-the-box. This may include, but is not limited to:

- The breach of pre-defined time thresholds for resolution
- Specific service or components linked to the incident
- Specific business units or users
- Specific business-periods

---

## Assignment & Notifications

### Incident Assignment

Incidents can be assigned to a support group or technician, manually and automatically, through predefined criteria (such as category, component, service, user, location, department, or a combination of these).

---

### Stakeholder Notifications

Notifications are triggered to identified stakeholders based on specific conditions in the incident record; this can include, but is not limited to:

- A specific status or change of status
- A change of priority
- Breach or impending breach of time expectations
- An assignment or reassignment of the incident
- Specific users, services, or components

---

### Resolution Notifications

Notifications of status updates and resolution can be sent to the service desk and the user.

---

## Service Agreements & Vendor Support

### Service Agreement Linking

Incidents can be linked or related to service and internal support agreements, to monitor and report response and resolution targets, as well as launch automatic notifications to predefined stakeholders.

---

### Vendor Support Integration

For incident support provided by a vendor, the following must be able to be done, at a minimum:

- Link the incident record to a vendor record or capture information about the vendor
- Link the incident record to a vendor support contract record or capture information about the contract and a specific warranty, if applicable

---

## User Portal & Self-Service

### User Portal Access

Users can access and review the status of their incidents via the portal/service catalog; this view should be restricted to the user recorded in the record, and also allow the user to update or add information to the incident throughout its life cycle.

---

## Incident Closure

### Problem and Change Record Launch

A problem record and a change record (as needed) can be launched from within the incident, linking the records together.

---

### Incident Closure Methods

Incident records can be closed in the following manners, as well as the flexibility for the client to determine which one or which combination they want to use. This may be different for the various incident models. This must include, at a minimum:

- The user can close the incident from the portal/service catalog (after resolution)
- The user can cancel the incident after it has been submitted by them via the portal
- The service desk can close the incident manually (after resolution)
- The incident can be systematically closed based on the elapsed time from the resolution
- The incident can be closed by the closure of the triggering alert (if the monitoring and alerting management functionality is applicable)

---

## Post-Incident Review

Post-incident reviews can be systematically triggered based on pre-defined criteria; the purpose of the review is to identify process and improvement opportunities; examples of this can include, but are not limited to:

- All major incidents, or incidents of other higher priority
- Incidents for certain services
- Incidents for certain users
- Incidents where the resolution targets were not met

---
