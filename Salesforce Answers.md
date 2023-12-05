# Salesforce Development Questions

## Q: How does the Approval Process work, and can you provide examples of scenarios where you have implemented it?

**A:** The Approval Process in Salesforce automates record approval by defining criteria and steps. Examples of implementation scenarios:
- **Deal Approval:** Require manager approval for opportunities exceeding a specific amount.
- **Expense Approval:** Automate approval for expenses above a set limit.

---

## Q: What is the role of Process Builder and Flows in Salesforce automation?

**A:**
- **Process Builder:** A point-and-click tool for automating processes, like updating fields or creating records.
- **Flows:** Declarative automation tools offering visual design for business logic.
  
---

## Q: How many types of flows are available, and what actions can be performed within flows?

**A:** There are two types of flows:
- **Screen Flows:** For user interaction.
- **Autolaunched Flows:** Triggered by processes or Apex.

Flows can perform actions such as creating/updating records, sending emails, and interacting with external systems.

---

## Q: Provide the syntax for writing an Apex class or validation rule to make a custom field, such as Master ID, mandatory.

**A:**
### Apex Class
```apex
public class CustomObjectValidator {
    public static void validateMasterId(String masterId) {
        if (String.isBlank(masterId)) {
            throw new CustomException('Master ID is required.');
        }
    }
}
```

### Validation Rule
```java
AND(
    ISBLANK(Master_Id__c),
    ISPICKVAL(Status, 'Active')
)
```

---

## Q: Share the syntax for creating a Lightning Web Component (LWC) if you have hands-on experience with it.

**A:**
### LWC Component
```html
<template>
    <lightning-card title="My Lightning Web Component">
        <!-- Component Content Goes Here -->
    </lightning-card>
</template>

import { LightningElement } from 'lwc';

export default class MyLWC extends LightningElement {
    // Component Logic Goes Here
}
```

---

## Q: Which files are included in a Lightning Bundle, and what is their significance in Salesforce development?

**A:** A Lightning Bundle typically includes the following files:
- **HTML file (.html):** Defines the structure and layout.
- **JavaScript file (.js):** Contains client-side logic.
- **XML file (.xml):** Metadata file.
- **CSS file (.css):** Optional styling file.

---

## Q: Scenario: You've added a new field to the Account object. How can you populate the field value within a Visualforce Page (VFP) template?

**A:** Use the following merge field syntax:
```html
{!Account.New_Field__c}
```

---

## Q: Explain how Visualforce Templates work, and provide a snippet of sample code to illustrate their usage.

**A:**
### Overview
Visualforce Templates generate dynamic documents, emails, or reports using merge fields and styling.

### Sample Code
```html
<apex:page standardController="Account" recordSetVar="accounts">
    <apex:repeat value="{!accounts}" var="acc">
        <p>Name: {!acc.Name}</p>
        <p>New Field: {!acc.New_Field__c}</p>
    </apex:repeat>
</apex:page>
```

---

## Q: Write a validation rule that makes specific fields mandatory based on certain conditions.

**A:**
```java
AND(
    ISPICKVAL(Type, 'Customer'),
    OR(
        ISBLANK(Primary_Contact__c),
        ISBLANK(Phone)
    )
)
```

This validation rule makes certain fields mandatory when the record type is "Customer."


## Q: Write a validation rule to make specific fields mandatory based on certain conditions.

**A:**
```java
AND(
    ISPICKVAL(Status, 'Approved'),
    OR(
        ISBLANK(Field1__c),
        ISBLANK(Field2__c)
    )
)
```
This rule makes `Field1__c` and `Field2__c` mandatory when the record status is "Approved."

---

## Q: How many ways are there to make fields mandatory in Salesforce?

**A:** There are four ways to make fields mandatory:
1. **Page Layouts:** Set the "Required" attribute on the page layout.
2. **Validation Rules:** Define rules to enforce mandatory fields.
3. **Process Builder:** Use criteria to update fields and make them required.
4. **Profile Settings:** Mark fields as required for specific user profiles.

---

## Q: What kind of approval processes have you worked on, and can you provide an example?

**A:** I have worked on various approval processes, such as:
- **Expense Approval:** Requires managerial approval for expenses exceeding a set limit.
- **Leave Request Approval:** Managerial approval for employee leave requests.

---

## Q: Scenario: If record A is approved, you need to send a notification to user B. Can you achieve this only through the approval process?

**A:** Yes, the approval process can trigger an outbound message, an email alert, or a custom notification to notify user B upon approval of record A.

---

## Q: How can you call Lightning Web Component (LWC) components?

**A:**
LWC components can be called in the following ways:
- **Imperatively:** Use JavaScript to create and place the component dynamically.
- **Declaratively:** Include the component in a parent component's HTML file.
- **Through App Builder:** Drag and drop the component onto a Lightning Page.
- **Programmatically:** Use events to communicate between components.

---

## Q: What are rule engines, and how can they be used in Salesforce?

**A:** Rule engines are systems that execute defined business rules. In Salesforce, Process Builder and Flows act as rule engines by allowing the creation of criteria-based processes and automation.

---

## Q: What is Workbench, and how can it be useful in Salesforce development?

**A:** Workbench is a web-based suite of tools for interacting with Salesforce organizations. It provides a set of utilities for working with metadata, querying data, executing REST APIs, and interacting with various Salesforce features.

---

## Q: Scenario: What happens if an email template is not available in the approval process?

**A:** If the email template is not available, the approval process won't be able to send notification emails. It's crucial to ensure that the required email templates are properly configured and available for use in the approval process.



## Workflow Path Configuration

**Q:** What is Workflow Path Configuration in Salesforce?

**A:** Workflow Path Configuration in Salesforce is a feature that allows you to define a guided process for users to follow when working with records. It helps in creating a more structured and guided user experience.

---

## Process Builder

**Q:** What is Process Builder in Salesforce?

**A:** Process Builder is a visual tool in Salesforce that allows users to automate business processes by creating processes with a user-friendly interface. It helps in streamlining complex workflows without requiring code.

---

## Approval Process

**Q:** What is an Approval Process in Salesforce?

**A:** An Approval Process in Salesforce is a combination of steps for a record to be approved or rejected. It involves defining criteria, actions, and approvers. It is commonly used for scenarios like record reviews, expense approvals, etc.

---

## Mandatory Fields

**Q:** In how many ways can you make a field mandatory?

**A:** There are several ways to make a field mandatory in Salesforce:

1. **Page Layouts:** Set the "Required" attribute on the page layout.

2. **Validation Rules:** Define rules to enforce mandatory fields.

3. **Process Builder:** Use criteria to update fields and make them required.

4. **Workflow Rules:** Create workflow rules to enforce field requirements.

**Q:** How can you make a field mandatory?

**A:** To make a field mandatory in Salesforce, you can follow these steps:

1. **Page Layouts:** Edit the page layout and mark the field as "Required."

2. **Validation Rules:** Create a validation rule that checks if the field is populated.

3. **Process Builder:** Use the "Update Records" action to set the field as required based on criteria.

4. **Workflow Rules:** Define a workflow rule to enforce the field requirement.

---

## Email Template in Approval Process

**Q:** What will happen if there is no email template selected in the approval process?

**A:** If no email template is selected in the approval process, users will not receive email notifications related to the approval process steps. Email templates are essential for notifying approvers and other stakeholders about the status of the approval.

---

## Validation Rules

**Q:** What are Validation Rules in Salesforce?

**A:** Validation Rules are used to ensure that data entered into records meets specific criteria before the records can be saved. They help in maintaining data accuracy and consistency by enforcing business rules.

---

## Apps in Salesforce

**Q:** What are Apps in Salesforce?

**A:** In Salesforce, an App is a collection of tabs that work as a unit to provide functionality to users. It is a way of organizing and delivering a set of related features and services in a unified user interface.


**Q: Have you worked on profiles and permission sets?**

**A:** Yes, I have experience working with profiles and permission sets in Salesforce. Profiles control users' access to objects, fields, and other features, while permission sets extend user permissions.

---

**Q: What are Sharing models in Salesforce?**

**A:** Sharing models in Salesforce define how records are shared among users. There are three standard sharing models: Private, Public Read Only, and Public Read/Write. Custom sharing rules can also be defined.

---

**Q: What are validation rules?**

**A:** Validation rules in Salesforce ensure that data entered into records meets specific criteria before the records can be saved. They help maintain data accuracy and consistency.

---

**Q: What is an approval process, flows, and process builder?**

**A:** 
- **Approval Process:** It's a set of steps for a record to be approved or rejected, often used for scenarios like expense approvals.
- **Flows:** Automate business processes by creating flows with a visual design interface.
- **Process Builder:** It's a visual tool used to automate business processes in Salesforce without the need for code.

---

**Q: When to use Trigger, Flows, and Process Builders?**

**A:** 
- **Triggers:** When complex logic or database operations are required.
- **Flows:** For visual, declarative automation of processes.
- **Process Builders:** For simpler, point-and-click automation with visual representation.

---

**Q: What are Sharing Rules?**

**A:** Sharing Rules are used to extend sharing access to records, allowing read or edit access to a particular group of users. They are used when you need to provide additional access beyond the organization-wide defaults.

---

**Q: Difference between Validation rule and Sharing rule?**

**A:**
- **Validation Rule:** Enforces data quality by validating input values.
- **Sharing Rule:** Extends record access to certain users or groups beyond default organization-wide settings.

---

**Q: Permission set and permission set group?**

**A:**
- **Permission Set:** Collection of permissions and settings that extend users' functional access.
- **Permission Set Group:** Bundles multiple permission sets together to grant a broader set of permissions.

---

**Q: How to restrict records with unwanted permissions?**

**A:** Use the appropriate combination of profiles, permission sets, and sharing rules to control user access and visibility to records.

---

**Q: Do permission sets override profile-level permissions, or do profile-level permissions override permission sets?**

**A:** Permission sets extend user permissions without overriding profile-level permissions. If there's a conflict, the most permissive settings prevail.

---

**Q: Profile-based access?**

**A:** Profile-based access in Salesforce involves assigning specific profiles to users, defining their permissions, object access, and system behavior.

---

**Q: How many types of Email templates are there?**

**A:** There are four types of Email templates in Salesforce: 
1. Text
2. HTML with letterhead
3. Custom HTML
4. Visualforce

