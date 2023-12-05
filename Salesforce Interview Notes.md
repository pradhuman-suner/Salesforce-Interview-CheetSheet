## Salesforce Admin Basics

### Cloud Computing
Cloud computing refers to the delivery of computing services over the internet, providing on-demand access to resources like storage, processing power, and applications.

### PaaS, SaaS, IaaS
- **PaaS (Platform as a Service):** Provides a platform for application development without managing the underlying infrastructure.
- **SaaS (Software as a Service):** Delivers software applications over the internet, eliminating the need for local installation.
- **IaaS (Infrastructure as a Service):** Offers virtualized computing resources on a pay-as-you-go basis.

### Sandbox in Salesforce
A Salesforce sandbox is a copy of an organization used for development, testing, and training without affecting the production environment. Types include Developer, Developer Pro, Partial, and Full.

### Object in Salesforce
In Salesforce, an object is a database table that stores data specific to the organization. Objects can be standard (built-in) or custom (user-defined).

### Object Relations in Salesforce
- **Lookup Relationship (LR):** Links objects without affecting deletion or security.
- **Master–Detail Relationship:** Creates a parent-child relationship with cascading behavior.
- **Junction Object:** Connects two master-detail relationships to model a many-to-many relationship.

### Master–Detail Relationship in Salesforce
A Master–Detail relationship establishes a parent-child connection between two objects, with the master object controlling certain behaviors and impacting related detail records.

### Junction Object in Salesforce
A junction object is used to connect two objects in a many-to-many relationship by utilizing two master-detail relationships.

### LR Fields in an Object
Salesforce allows creating up to 25 Lookup Relationship fields on an object.

### Roll-up Summary Field
A Roll-up Summary field in Salesforce performs calculations on related records and displays the result on a master record in a Master–Detail relationship.

### Ways to Create Roll-up Summary Field
Roll-up Summary fields can be created using point-and-click tools like the Setup menu or declaratively through the Schema Builder.

### Field Dependency
Field dependency in Salesforce allows controlling the visibility of a field based on the value of another field.

### Role vs. Profile
- **Role:** Defines a user's position in the hierarchy, determining access to records owned by users below them.
- **Profile:** Specifies a user's permissions and how they view records, including page layouts and field-level security.

### Permission Sets
Permission sets in Salesforce provide additional permissions to users without changing their profiles.

### Muting Permission Set in Permission Set Group
Muting a permission set in a permission set group suppresses specific permissions granted by other permission sets in the same group.

### Ways to Share a Record
Records in Salesforce can be shared through manual sharing, sharing rules, and criteria-based sharing.

### Audit Fields in Salesforce
Audit fields, such as Created By, Created Date, Last Modified By, and Last Modified Date, track changes to records.

### Audit Trail
The Audit Trail in Salesforce logs changes made by administrators, providing a history of setup changes.

### Queue in Salesforce
A queue in Salesforce is a group of users who can own or take ownership of records manually or through assignment rules.

### Public Group
A public group in Salesforce is a collection of users, roles, roles and subordinates, or other groups, used for sharing records or setting up group email.

### Static vs. Dynamic Dashboards
- **Static Dashboards:** Have a fixed layout and display data as it was when the dashboard was created.
- **Dynamic Dashboards:** Allow users to interact with the data, applying filters and changing the displayed information.

### Types of Reports in Salesforce
Reports in Salesforce include Tabular, Summary, Matrix, and Joined reports, providing various ways to present and analyze data.

### Report Type
A report type in Salesforce defines which objects and fields are available when creating a report.

### WhoId and WhatId in Activities
- **WhoId:** Represents a lead or a contact in activities.
- **WhatId:** Represents an object (such as an opportunity or case) in activities.

### Bucket Field in Reports
A bucket field in Salesforce allows grouping of report data based on ranges defined by the user.

### Ways to Clean Data in Salesforce
Data can be cleaned in Salesforce through tools like Data Loader, Excel, and by implementing validation rules.

### Import Wizard vs. Data Loader
- **Import Wizard:** A web-based tool for importing data with a simplified interface.
- **Data Loader:** A desktop application for bulk data import and export with more advanced features.

### "Data Skew" in Salesforce
Data skew refers to situations where a small number of records disproportionately impact performance, often seen in scenarios like ownership skew or lookup skew.

### Cascade Deletion
Cascade deletion in Salesforce automatically deletes related child records when the parent record is deleted.

### Flow
Flow in Salesforce is a tool for automating business processes by collecting, updating, and creating records.

### Types of Flows in Salesforce
Types of flows include Screen Flows, Auto-launched Flows, and Lightning Flows, each serving different automation purposes.

### Global Variables in Formula and Validation Rules
Global variables like $User, $Profile, and $Record facilitate dynamic calculations and validations in formulas.

### Special Permission for Editing Read-Only Fields
The "Modify All Data" permission grants users the ability to edit read-only fields.

### Object-Specific Action vs. Global Actions
- **Object-Specific Action:** Associated with a specific object and appears in the object's page layout.
- **Global Actions:** Can be used from any page and are not tied to a specific object.

### Impact Point Before Deleting a Role
Check for any active sharing rules or manual shares that reference the role.

### Making a1 Parent of a2 After Initial Configuration
Salesforce does not allow changing the parent in a Master–Detail relationship once records exist.

### Passing Record ID to Screen Flow
Use a URL parameter or a variable assignment to pass the current record ID to a screen flow.

### Checking Salesforce Release Version
View the "Release Information" in the Salesforce Setup menu.

### Big Object
A big object in Salesforce is designed for storing and managing large volumes of data. An example is the "Event" standard big object.

### Using Formula Field in Roll-Up Summary Calculation
Formula fields cannot be used directly in roll-up summary calculations across objects.

### Default Value on Unadded Field in Cloned Record
The new record will inherit the default value even if the field is not on the page layout.

### Considerations While Deleting an Approval Process
Ensure that no records are pending approval, and deactivate the process before deletion.

### Lead Merging
Lead merging combines duplicate lead records, preserving the best information.

### Apex Hammer
"Apex Hammer" is not a recognized term in Salesforce. It might be a custom tool or code named by a specific organization.

### Converting 15-Digit Record ID to 18-Digit ID
Use the CASESAFEID function in formulas to convert 15-digit IDs to 18-digit format.

### Hard Deleting Records Using Data Loader
Yes, data loader provides an option for hard deletion when performing data operations.

### Showing Validation Errors in Screen Flow
Validation errors can be displayed by configuring fault connectors in a screen flow.

### Creating Report on Custom Object Issue
Ensure the object has records, the user has the "View All Data" permission, and the object is not deleted or in the recycle bin.

### Possible Statuses of a Permission Set Group
Statuses of a permission set group can be "Active," "Inactive," or "

Deleted."

### Enabling Email Approval Response
Email approval responses can be enabled by checking the "Allow Email Approval Response" checkbox in the approval process setup. Response keywords include "Approve," "Approve with Changes," and "Reject."

### Option Not Available for Creating List Custom Settings
Ensure that the "Custom Settings" feature is enabled in the Salesforce organization.

### Permission to View Converted Leads
Users need the "View All Data" or "View All" permission on leads to view converted leads.

### Issue with Converting a Master Detail Relationship Field
Ensure that there are no child records in the Master–Detail relationship, as changing the field type is not allowed when records exist.

### User Unable to Create Campaigns
Check the user's profile and permission sets to ensure they have the necessary permissions to create campaigns. Also, verify that the user's role allows access to the campaigns.

### Deleting a Public Group
When you delete a public group, the group is permanently removed, and any associated sharing rules or permissions are also deleted.

### Deleting a Queue
When you delete a queue, the queue is removed, and any associated records that were owned by the queue are reassigned to the users who were members of the queue.

## Salesforce Dev 


### Sandbox in Salesforce
A Salesforce sandbox is a copy of an organization used for development, testing, and training without affecting the production environment. Types include Developer, Developer Pro, Partial, and Full.

### Cloud Computing
Cloud computing refers to the delivery of computing services over the internet, providing on-demand access to resources like storage, processing power, and applications.

### IaaS (Infrastructure as a Service)
IaaS offers virtualized computing resources over the internet. Users can rent virtual machines and other resources on a pay-as-you-go basis.

### PaaS (Platform as a Service)
PaaS provides a platform for application development without managing the underlying infrastructure.

### SaaS (Software as a Service)
SaaS delivers software applications over the internet, eliminating the need for local installation.

### Object Relationship in Salesforce
Types of object relationships in Salesforce include Lookup Relationship, Master–Detail Relationship, and Junction Object.

### Junction Object in Salesforce
A junction object connects two objects in a many-to-many relationship, utilizing two master-detail relationships.

### Role vs. Profiles
- **Role:** Defines a user's position in the hierarchy, determining access to records owned by users below them.
- **Profile:** Specifies a user's permissions and how they view records, including page layouts and field-level security.

### Sharing in Salesforce
Salesforce provides various ways for sharing, including manual sharing, sharing rules, and criteria-based sharing.

### Sharing Rules
Sharing rules in Salesforce automate the sharing of records based on criteria.

### Manual Sharing
Manual sharing allows users to manually grant access to individual records.

### Apex Sharing
Apex sharing involves programmatically sharing records using Apex code.

### Flow in Salesforce
Flow in Salesforce is a tool for automating business processes by collecting, updating, and creating records.

### When to use Flow vs. Apex
Use Flow for declarative automation and Apex for more complex, programmatic scenarios.

### Best Practices for Salesforce Flow
Best practices for Salesforce Flow include modular design, using subflows, and considering governor limits.

### Apex in Salesforce
Apex is a programming language in Salesforce used for building custom business logic.

### When to use Apex over Flow
Use Apex when complex logic, bulk processing, or integrations are required.

### Apex Best Practices
Apex best practices include bulkifying code, adhering to governor limits, and using trigger frameworks.

### Apex Trigger
Apex Trigger is code that runs before or after specific data manipulation events occur on records in Salesforce.

### When to use Apex Trigger
Use Apex Trigger when you need to perform custom actions based on record changes.

### Apex Trigger Handler Pattern
The Apex Trigger Handler pattern separates trigger logic into handler classes for better organization and maintainability.

### Apex Trigger Framework
An Apex Trigger Framework provides a structured approach to handling triggers. Examples include Trigger Handler and Trigger Factory.

### Async Apex in Salesforce
Async Apex in Salesforce allows processing tasks asynchronously. Ways include Batch Apex, Queueable Apex, and Scheduled Apex.

### Batch Job in Salesforce
A Batch Job in Salesforce is a type of Async Apex that processes large sets of data in small, manageable chunks.

### Stateful vs. Stateless Batch Job
A stateful batch job retains state across transactions, while a stateless batch job does not.

### Mixed DML
Mixed DML refers to performing DML operations on different types of objects in a single transaction.

### Lightning Data Service
Lightning Data Service is a standard set of methods in Lightning components for accessing and modifying Salesforce data.

### Communication Between Lightning Web Components
Lightning Web Components communicate through events, including standard events, component events, and application events.

### Calling Apex Class in Lightning Web Component
Apex classes can be called in Lightning Web Components using imperative or wire service methods.

### Basic Difference Between Application Event and Component Event in Aura Component
- **Application Event:** Communicates between components across the entire application.
- **Component Event:** Communicates between parent and child components.

### Lightning Messaging Service
Lightning Messaging Service provides a standard communication channel between components on a Lightning page.

### Lazy Loading in LWC
Lazy loading in LWC defers the loading of JavaScript resources until they are needed.

### Design Attributes in Lightning Web Components
Design attributes in Lightning Web Components allow developers to configure components in the Lightning App Builder.

### Web Services
Web services are a standard way of integrating web-based applications over a network.

### SOAP vs. REST
- **SOAP (Simple Object Access Protocol):** Protocol for exchanging structured information in web services.
- **REST (Representational State Transfer):** Architectural style for designing networked applications.

### Enterprise WSDL vs. Partner WSDL
- **Enterprise WSDL:** Exposes all objects and actions for a specific Salesforce organization.
- **Partner WSDL:** Provides a loosely coupled connection to any Salesforce organization.

### Integration Patterns
Integration patterns define best practices for connecting systems and sharing data across applications.


## Salesforce Integration Basics

### 1. Integration
Integration refers to the process of connecting different systems and enabling them to work together, often sharing data and functionality.

### 2. Web Services
Web services are standardized protocols that allow different software applications to communicate with each other over the internet.

### 3. JSON vs. XML
- **JSON (JavaScript Object Notation):** Lightweight data interchange format. 
- **XML (eXtensible Markup Language):** Extensible markup language for encoding documents.

### 4. REST API
REST (Representational State Transfer) API is an architectural style for building web services. It uses standard HTTP methods for communication.

### 5. SOAP API
SOAP (Simple Object Access Protocol) API is a protocol for exchanging structured information in web services. It uses XML for message formatting.

### 6. SOAP vs. REST
- **SOAP:** Protocol with strict standards, often used in enterprise environments.
- **REST:** Lightweight protocol, widely used for web and mobile applications.

### 7. Salesforce Integration Options
Salesforce offers various integration options, including REST API, SOAP API, Streaming API, Salesforce Connect, and more.

### 8. WSDL
WSDL (Web Services Description Language) is an XML format that describes the functionality offered by a web service.

### 9. SoapUI
SoapUI is an open-source tool for testing web services. It supports both SOAP and RESTful services.

### 10. Enterprise WSDL vs. Partner WSDL
- **Enterprise WSDL:** Exposes all objects and actions for a specific Salesforce organization.
- **Partner WSDL:** Provides a loosely coupled connection to any Salesforce organization.

### 11. Integration Patterns
Integration patterns are best practices and design principles for connecting systems and sharing data.

### 12. Integration Patterns in Salesforce
Different integration patterns in Salesforce include Request and Reply, Fire and Forget, Batch Data Synchronization, and Remote Process Invocation.

### 13. Remote Site Settings
Remote Site Settings in Salesforce allow external websites to communicate with Salesforce using HTTP callouts.

### 14. Connected App
A Connected App is an integration framework that enables external applications to connect to Salesforce securely.

### 15. OAuth
OAuth is an open standard for access delegation commonly used for authentication and authorization.

### 16. OAuth 2.0 Authorization Flows
Different OAuth 2.0 authorization flows in Salesforce include Authorization Code Flow, Implicit Flow, Resource Owner Password Credentials Flow, and Client Credentials Flow.

### 17. JWT Flow in Salesforce
JWT (JSON Web Token) Flow is an OAuth 2.0 flow in Salesforce that allows a connected app to obtain access tokens.

### 18. Web Service Flow in Salesforce
Web Service Flow in Salesforce is a type of integration flow used to connect with external web services.

### 19. Named Credentials
Named Credentials in Salesforce store authentication details for external services, enhancing security.

### 20. OpenID Connect
OpenID Connect is an authentication layer on top of OAuth 2.0, providing identity verification.

### 21. Difference Between OpenID and OAuth
- **OpenID:** Identity layer protocol for authentication.
- **OAuth:** Authorization framework for secure access.

### 22. Streaming API
Streaming API in Salesforce allows real-time streaming of data updates to subscribed clients. Mechanisms include Push Topic, Generic Events, and Platform Events.

### 23. Change Data Capture
Change Data Capture in Salesforce tracks changes to records, enabling efficient synchronization with external systems.

### 24. Tooling API
Tooling API in Salesforce provides a way to interact with the metadata of your organization. It's often used for development and testing purposes.

### 25. Salesforce Connect
Salesforce Connect allows you to access and display data from external systems directly within Salesforce.

### 26. REST API Composite Resources
Composite Resources in Salesforce REST API allow you to perform multiple operations in a single request, improving efficiency in data manipulation.

## Salesforce Trigger Basics

### What is Trigger in Salesforce?
A trigger in Salesforce is a piece of Apex code that is executed before or after records are inserted, updated, deleted, or undeleted in Salesforce.

### What are the Two Types of Triggers in Salesforce?
The two types of triggers in Salesforce are "Before Triggers" and "After Triggers."

### What is the Use of Trigger Class in Salesforce?
A trigger class in Salesforce is used to hold the logic that needs to be executed in response to trigger events.

### What are Different Events Available in Triggers?
Different events in triggers include "Before Insert," "Before Update," "Before Delete," "After Insert," "After Update," "After Delete," and "After Undelete."

### When Should You Use Trigger or Automation?
Use triggers for complex business logic, validations, or when you need to perform operations on related records. Use declarative automation (e.g., Process Builder) for simpler tasks.

### Best Practices and Considerations for Triggers?
- Keep triggers focused on a single concern.
- Bulkify your code to handle bulk data.
- Avoid using SOQL queries inside loops.
- Handle trigger recursion to prevent unwanted behavior.

### How Many Times Does Trigger Execute on an Upsert Event?
A trigger executes once per batch in an upsert event.

### How Many Times Does Trigger Execute on a Merge Event?
A trigger executes once per merge operation.

### Order of Execution for Trigger
1. Before Triggers.
2. System Validation Rules.
3. Custom Validation Rules.
4. After Triggers.
5. Assignment Rules.
6. Auto-Response Rules.
7. Workflow Rules.
8. Processes.
9. Escalation Rules.
10. Entitlement Rules.
11. Roll-up Summary Fields.
12. Criteria-Based Sharing Rules.
13. Territory Assignment Rules.

### When Will You Choose Before Event and When Will You Choose After Event?
- Use "Before" events when you need to validate or modify record data before it's committed to the database.
- Use "After" events when you need to perform additional actions after the record has been committed.

### What is the Difference Between Trigger.New and Trigger.newMap?
- `Trigger.New:` Represents a list of sObjects before they are saved to the database (available in "Before" events).
- `Trigger.newMap:` Represents a map of IDs to sObjects before they are saved to the database (available in "Before" events).

### When Should You Use Trigger.Old?
Use `Trigger.Old` to access the old version of records in "Before Update" and "After Update" triggers.

### How to Avoid Recursion in Trigger?
To avoid recursion, use static variables or a custom setting to keep track of whether the trigger has already executed in the current transaction.

### How to Make a Callout from Trigger?
Making a callout from a trigger is generally not recommended due to governor limits. Instead, use an asynchronous method like Queueable or @future.

### Can We Call a Batch Job from Trigger?
Technically, you can call a batch job from a trigger, but it's generally not recommended due to governor limits and potential performance issues.

### What is Trigger Handler Pattern?
The Trigger Handler Pattern is an approach to organize and structure trigger logic by separating it into handler classes. This pattern improves code readability, maintainability, and reusability.

### Have You Used Any Trigger Framework in Salesforce?
Yes, trigger frameworks like Trigger Framework by Kevin O'Hara or fflib Apex Common by Andrew Fawcett provide a structured way to handle triggers.

### Difference Between Validation Rules and Triggers?
- **Validation Rules:** Declarative rules used to ensure data quality before saving records. Executed on the database server.
- **Triggers:** Programmatic logic written in Apex that allows more complex business rules and actions to be performed during record processing. Executed on the application server.



# Notes

# Salesforce Notes

## Objects
- **Standard Objects:** Salesforce provides a set of standard objects for common Customer Relationship Management (CRM) needs. Examples include Account, Contact, Lead, Opportunity, Case, and Task.
  
- **Custom Objects:** Organizations can create custom objects to store data specific to their unique needs. Custom objects can have custom fields and relationships.

## Types of Relationships
1. **Lookup Relationship:** Establishes a loose association between two objects, often used in a many-to-one relationship. Parent deletion does not automatically delete child records.

2. **Master-Detail Relationship:** Creates a strong relationship used in a one-to-many relationship. Deletion of master records automatically deletes related detail records.

3. **Self-Relationship:** Connects records within the same object, useful for modeling hierarchies like manager-to-subordinate relationships.

4. **Many-to-Many Relationship (Junction Object):** Salesforce lacks a native many-to-many relationship. Junction objects with two lookup relationships model complex many-to-many relationships.

## Order of Execution (Salesforce)
1. **System Validation**
2. **Before Record-Triggered Flow**
3. **All Before Triggers**
4. **Custom Validation**
5. **Duplicates Rule**
6. **All After Triggers**
7. **Assignment Rule**
8. **Auto Response Rule**
9. **Workflow Rule**
10. **Escalation Rule**

## Roles & Profile
- **Roles:** Record-level access controls determining visibility for specific users.

- **Profile:** Object and field-level access controls determining create, read, edit, or delete permissions.

## Permission Sets and Permission Set Groups
- **Permission Set:** Collection of settings and permissions assigned to individual users or groups, extending or modifying profile permissions.

- **Permission Set Group:** Collection of permission sets providing comprehensive permissions for users needing a combination of different sets.

## Record-Level Security
- **Organization-Wide Sharing Defaults:** Control default access to records for users who do not own them.

- **Sharing Rules:** Ownership-based sharing rules (role, role-and-subordinate, public group) and criteria-based sharing rules to grant access.

- **Manual Sharing:** Mechanism to individually share records with others using the Sharing button on the record details page.

## Automation Tools in Salesforce
### Workflow
- Automate internal procedures and processes using if/then statements based on record creation and updates.
  
#### Workflow Actions
- Email Alert
- Task
- Outbound Message
- Field Update

### Process Builder
- Automate tasks, emails, and updates. Supports record change, event, and invocable processes.

### Approval Process
- Defined steps for approving records, often involving multiple stakeholders.

### Flow
- Graphical tool for automating business processes, recommended over Process Builder for complex scenarios.

## User Management
- **Deleting User:** Users cannot be deleted but can be frozen or deactivated.

## Security in Salesforce
- **Record-Level Security (Organization-Wide Sharing Defaults):** Controls default access to records for users who do not own them.

- **Record-Level Security (Sharing Rules):** Ownership-based sharing rules (role, role-and-subordinate, public group) and criteria-based sharing rules to grant access.

- **Record-Level Security (Manual Sharing):** Allows users to manually share individual records with others.

## Additional Topics
- **Field-Level Security:** Controls access to fields in objects based on profiles.

- **Object-Level Security:** Determines the visibility and permissions for objects based on profiles.

- **Apex Triggers:** Code that executes before or after records are inserted, updated, or deleted.

- **Batch Apex:** Allows for the processing of large data sets through the use of batch jobs.


## Apex

### What is Apex?
Apex is a strongly typed, object-oriented programming language used in Salesforce development. Developers use Apex to execute flow and transaction control statements on Salesforce servers, adding business logic to various system events.

### Best Practices of Apex
1. **Bulkify Your Code:** Ensure your code can handle bulk operations efficiently.
2. **Avoid DML/SOQL Queries in Loops:** Performing DML or SOQL queries inside loops can lead to performance issues.
3. **Avoid Hard-coded IDs:** Dynamically reference IDs to enhance code flexibility.
4. **Use a Single Trigger per SObject Type:** Maintain a single trigger for each Salesforce object to keep code organized.
5. **Avoid Nested Loops:** Limit the use of nested loops to prevent performance degradation.
6. **Have a Naming Convention:** Use a consistent naming convention for variables, classes, and methods.
7. **Avoid Business Logic in Triggers:** Move business logic to separate classes or triggers for better maintainability.
8. **Code Coverage Above 75%:** Aim for sufficient test coverage to deploy Apex code.

### What is a Trigger?
A trigger in Salesforce is Apex code that executes before or after changes to Salesforce records, such as insertions, updates, or deletions.

### Types of Trigger Events
1. **Before Trigger:** Used to update or validate record values before saving to the database.
2. **After Trigger:** Executes after changes to record values, allowing manipulation of data from the inserted records.

### Context Variable (Trigger)
The `System.Trigger` class contains implicit variables providing information about the runtime context of the trigger.

### Types of Context Variables
1. `isExecuting`
2. `isInsert`
3. `isUpdate`
4. `isDelete`
5. `isBefore`
6. `isAfter`
7. `isUndelete`
8. `new`
9. `newMap`
10. `old`
11. `oldMap`

### Best Practices of Triggers
1. **One Trigger per Object:** Maintain one trigger per Salesforce object for simplicity.
2. **Logic-Less Trigger:** Move logic to separate handler methods to enhance readability.
3. **Context-Specific Handler Methods:** Create methods for specific trigger events for modular code.
4. **Avoid SOQL Query inside for Loop:** Minimize SOQL queries inside loops to avoid hitting governor limits.
5. **Avoid Hardcoding IDs:** Dynamically reference IDs for better code flexibility.
6. **Avoid Nested For Loop:** Minimize nested loops to improve performance.
7. **Avoid DML Inside For Loop:** Execute DML operations outside loops for efficiency.
8. **Bulkify Your Code:** Ensure your code handles bulk data operations effectively.
9. **Enforced Sharing in Salesforce:** Check and enforce sharing rules as needed.
10. **Use @future Appropriately:** Use asynchronous processing for long-running operations.
11. **Use WHERE Clause in SOQL Query:** Optimize SOQL queries with WHERE clauses.
12. **Use Test-Driven Development:** Write test classes to ensure robust code.

### Types of Apex
1. **Synchronous Apex:** Entire Apex code is executed in a single go.
2. **Asynchronous Apex:** Executes when resources are available, allowing for long-running operations.

### Types of Asynchronous Apex
1. **Batch Apex:** For long-running jobs with large data volumes, executed in batches.
2. **Schedule Apex:** Schedules an Apex class to run on a specific schedule.
3. **Queueable Apex:** Initiates long-running operations and allows chaining of jobs.
4. **Future Method:** Executes asynchronously to prevent delaying an Apex transaction.

### Insert and Database.Insert
- **Insert:** DML statement that stops execution if an error occurs during a bulk operation.
- **Database.Insert:** DML database method that inserts as many records as possible, even if an error occurs.

### DML and Mixed DML
- **Mixed DML Operation Error:** Occurs when performing DML operations on setup and non-setup objects in a single transaction.

### Name Credentials
A named credential specifies the URL of a callout endpoint and its required authentication parameters in one definition.

### External ID
An external ID is a custom field with the External ID attribute, containing unique identifiers from a system outside of Salesforce.

### Public Group vs. Queue
- **Public Group:** A team or group of linked users used for sharing data.
- **Queue:** Used for assigning records to a group of users, allowing any member to work on the record.

### Custom Metadata and Custom Setting
- **Custom Metadata:** Defines custom data types for applications.
- **Custom Setting:** Stores custom data, allowing reusable application configurations.

## Salesforce Governor Limits

Governor limits in Salesforce are designed to ensure the effective use of resources on the Force.com multi-tenant platform. These limits include:
- Maximum number of records retrieved using query locator in a batch: 50 million records.
- Maximum number of batch executions per 24 hours: 250,000.

## SOQL and SOSL

### Difference between SOQL and SOSL
- **SOQL (Salesforce Object Query Language):** Used to query records from a single object at a time.
- **SOSL (Salesforce Object Search Language):** Used to search records across multiple objects simultaneously.

### SOQL Examples
- Parent-to-Child (Standard Object):
  ```sql
  SELECT Name, Phone, (SELECT Name, Phone FROM Contacts) FROM Account
  ```
- Parent-to-Child (Custom Object):
  ```sql
  SELECT Name, (SELECT Name FROM CustomObjectA__c) FROM CustomObjectB__c
  ```
- Child-to-Parent (Standard Object):
  ```sql
  SELECT Contact.FirstName, Contact.Phone, Account.Name, Account.Phone FROM Contact
  ```
- Child-to-Parent (Custom Object):
  ```sql
  SELECT Id, Name, Org__r.Name FROM CustomObject__c WHERE Org__r.CreatedBy.LastName LIKE 'Muj%'
  ```

### SOSL Examples
- Basic Syntax:
  ```sql
  FIND {John} IN ALL FIELDS RETURNING Object__c
  ```
- Returning Specific Fields:
  ```sql
  FIND {John} IN ALL FIELDS RETURNING Object__c(Name)
  ```
- Returning Multiple Objects:
  ```sql
  FIND {John} IN ALL FIELDS RETURNING Object1__c, Object2__c
  ```
- Advanced SOSL:
  ```sql
  FIND {John} IN ALL FIELDS RETURNING Object__c(FirstName), Object2__c(Price__c WHERE Price__c > 1000 ORDER BY Price__c)
  ```

## Record Type

Salesforce Record Types group records of a particular object, allowing different page layouts, fields, required fields, and picklist values. Benefits include reducing field clutter and improving data quality.

## Batch Size

- **Default:** 200
- **Max:** 2000
- **Min:** 1

## Additional Topics

### What is Setup Object?
Setup objects affect user access to records. Examples include ObjectPermissions, PermissionSet, UserRole, etc.

### What is Non-Setup Object?
Non-setup objects store and manipulate data, such as standard or custom objects like Account, Contact, or custom objects created by administrators.

### What is Named Credential?
A named credential specifies the URL and authentication parameters for callout endpoints, simplifying authenticated callouts.

### What

 is External ID?
An external ID is a custom field containing unique record identifiers from a system outside of Salesforce.

### What is the Difference Between Public Group and Queue?
- **Public Group:** A team or group of linked users for sharing data.
- **Queue:** Used for assigning records to a group of users, allowing any member to work on the record.

### What is Custom Metadata and Custom Setting?
- **Custom Metadata:** Defines custom data types for applications.
- **Custom Setting:** Stores custom data, allowing reusable application configurations.

### Salesforce Governor Limits
Governor limits are designed to ensure the effective use of resources on the Force.com multi-tenant platform. These include maximum records retrieved in a batch and maximum batch executions per 24 hours.

### SOQL and SOSL
- **SOQL (Salesforce Object Query Language):** Used for querying records from a single object.
- **SOSL (Salesforce Object Search Language):** Used for searching records across multiple objects.


## Reports

Reports in Salesforce provide tabular or tabular-like representations (with optional charts) of records meeting specific criteria, answering specific questions. There are different types of reports:

- **Tabular Reports:** Simplest form, displaying records in a spreadsheet-like format. Suitable for creating dashboards but cannot be used to create report charts.

- **Summary Reports:** Group records based on conditions, providing subtotals and report charts. Ideal for dashboard creation, e.g., showing opportunities grouped by each stage.

- **Matrix Reports:** Group records both row-wise and column-wise, offering more detailed insights. Supports dashboards, report charts, bucket fields, and formulas.

- **Joined Reports:** Contain multiple blocks with customizable data based on filter conditions, allowing a 360-degree view of data.

## Dashboards

Dashboards in Salesforce are graphical representations of reports. They provide a visual snapshot of key metrics and performance indicators, displaying data from source reports.

## Validation Rule

Validation rules ensure that data entered in a record meets specified standards before the user can save the record. These rules contain formulas or expressions that evaluate data in one or more fields, returning a value of "True" or "False."

## Assignment Rule

Assignment rules dictate to whom a lead or case is assigned based on specified criteria within Salesforce. Different rules may exist for various purposes, such as importing leads or handling web-generated leads.

## Escalation Rule

An escalation rule automatically reroutes a case and notifies a user if the case remains open beyond a defined time period. It helps ensure timely resolution by escalating cases based on specific criteria.

## Salesforce Licenses and Editions

Salesforce licenses provide metadata descriptions of features and services available in your organization. Editions refer to the different versions of Salesforce, each tailored to specific needs, with sandboxes serving as isolated copies for testing and training.

## With Sharing and Without Sharing in Apex

- **With Sharing:** Enforces record permissions based on the sharing rules of the current user. It does not enforce object or field-level security permissions.

- **Without Sharing:** Classes declared with this keyword are executed in system mode, ignoring record-level sharing permissions.

## Stateful and Stateless in Asynchronous Apex

- **Stateful:** Retains information about the state of a process across multiple transactions or method calls.

- **Stateless:** Does not retain information about the state of a process across multiple transactions or method calls.

## Calling Apex Class in Flow and Process Builder

By using the `@InvocableMethod` annotation.

## Calling Apex Class in Lightning Web Components (LWC)

By using `@AuraEnabled(cacheable=true)`.

## Shared Object in Salesforce

A shared object in Salesforce allows defining four pieces of information: the record being shared, the user or group with whom the object is shared, the permission level granted, and the reason for granting sharing access.

## Salesforce Audit

Salesforce audit involves a thorough inspection of the platform or specific tools to ensure seamless and efficient functioning. It helps identify issues and take preventive measures for optimal system performance.

## Difference Between Table and Database.Table

- **Table:** A structured collection of data organized into rows and columns.
  
- **Database.Table:** A collection of related tables along with associated objects (e.g., indexes, views, procedures) and metadata within a database.

## Visualforce Framework

The Visualforce framework in Salesforce allows developers to build sophisticated, custom user interfaces natively hosted on the Lightning Platform. It includes a tag-based markup language, similar to HTML, and server-side "standard controllers" for basic database operations.

- **Standard Controllers:** Default controllers provided by Force.com, offering logic and functionality used in standard Visualforce pages. No Apex code is required for standard controllers.

- **Custom Controllers:** Developers can write their own Apex controller classes for different logic and functionality, providing a customized approach. Custom controllers require custom Apex code.

- **Extension Controllers:** Combining both standard and custom controller functionalities, extension controllers extend or override standard controllers with additional custom Apex code.

## Integration

Salesforce Integration involves bringing two or more systems together to streamline separate processes. There are different integration methods:

1. **REST API:** Focuses on data-based operations such as GET, POST, PUT, PATCH, and DELETE. Suitable for web or mobile applications, using XML or JSON data formats.

2. **SOAP API:** Best for system-to-system integrations, back-end system communication, and applications requiring formal hand-off (contracts) between the API and consumer. Uses XML for structured payloads.

## Lightning Web Components (LWC)

Lightning Web Components revolutionize web application development on the Salesforce platform. They provide a modern, efficient, and developer-friendly framework with a component-based architecture.

**Lifecycle of LWC:**

1. **Constructor():** Invoked when the instance of the component is created, similar to the init() method in Aura components.

2. **ConnectedCallback():** Invoked when the component is inserted into the DOM.

3. **RenderedCallback():** Invoked when a component is completely rendered on the UI.

4. **DisconnectedCallback():** Activated when a component is removed from the DOM, suitable for tidying tasks like removing event listeners.

5. **Error Callback:** Catches errors in a component's lifecycle or its children and can display user-friendly error messages.

**Decorators of LWC:**

Three types of decorators are used in LWC:

1. **@wire:** Used for reactive wire services to read Salesforce data. Specifies a wire adapter or an Apex method.

2. **@api:** Used to expose public properties and methods, defining the API for a component.

3. **@track:** Used to observe changes to field values, triggering component rerenders when a field's value changes.

**Note:** Be cautious not to call a wire from the wire decorator.


## Lightning Data Service (LDS)

Lightning Data Service is a centralized data caching mechanism that enables CRUD operations on a record without making server-side Apex calls in Lightning Web Components (LWC). Key components built on LDS include:

- **lightning-record-form:** A form with standard Lightning UI for creating, viewing, or editing a record.
  
- **lightning-record-edit-form:** A form to create a record with specified fields or update fields in an existing record.
  
- **lightning-record-view-form:** A form to display specific field data of a record in read-only mode.

## Lightning Message Service (LMS)

LMS is introduced to facilitate event communication between unrelated LWC components on the same Lightning page. It replaces the obsolete pubsub pattern and involves creating a message channel to define variables or fields for data storage during event communication. Steps for LMS integration:

1. **Create a Message Channel:**
   - Create a folder "messageChannels" under force-app\main\default.
   - Create a file "messagingChannel.messageChannel-meta.xml."

2. **Publish Events:**
   - Import publish and MessageContext from LMS.
   - Use the publish method to send events to the Lightning Message Service.

3. **Subscribe to Events:**
   - Import subscribe and MessageContext from LMS.
   - Use the subscribe method to capture events in different LWC components.

## Navigation Service in LWC

Navigation Service allows developers to navigate to various Salesforce pages, objects, list views, etc. It uses a PageReference, a JavaScript object providing details of page type, attributes, and page state. Example of using NavigationMixin:

```javascript
import { NavigationMixin } from 'lightning/navigation';

export default class SampleNavigationService extends NavigationMixin(LightningElement) {
  // Your component logic here
}
```

## Imperative Method in LWC

While wire calls automatically update data from the server, imperative calls involve explicitly calling an Apex method using JavaScript. It retrieves data from the server only when needed, such as on page load or button click. Syntax example:

```javascript
// Sample imperative Apex call
import fetchData from '@salesforce/apex/Controller.fetchData';

fetchData({ params })
  .then(result => {
    // Handle the result
  })
  .catch(error => {
    // Handle errors
  });
```

## Recursive Trigger

A recursive trigger occurs when the same trigger is executed multiple times, updating a record repeatedly due to automation. This can lead to hitting Salesforce Governor Limits.

## Recursive Workflow

A recursive workflow rule occurs when the "Re-evaluate Workflow Rules after Field Change" checkbox is enabled in the Field Update of a workflow rule. This can trigger other workflow rules on the same object if their entry criteria are satisfied.

## Bucket Field

The Bucket Field in Salesforce reporting allows for rapid categorization of values without creating a custom formula field. It is a custom category created in a report and documentation tool.

## DataLoader

Data Loader is a client application for bulk import/export of data in Salesforce. It reads, extracts, and loads data from CSV files or a database connection.

## Dashboards in Salesforce

Salesforce has two types of dashboards: Static Dashboards and Dynamic Dashboards.

- **Static Dashboards:** Appear the same to all viewers based on their profile and permissions.

- **Dynamic Dashboards:** Customized for each viewer, regardless of their permissions. They allow viewers to see data they might not have direct permission to view.

**Limits:**
- Enterprise Edition: 5 dynamic dashboards
- Unlimited and Performance Editions: 10 dynamic dashboards
- Developer Edition: 3 dynamic dashboards

## Trigger-Based Scenarios

**Scenario 1:**
When a case is created with the origin as email, set status as new and priority as medium.

```apex
trigger CaseOrigin on Case (before insert) {
  for (Case c : Trigger.new) {
    if (c.Origin == 'email') {
      c.Status = 'new';
      c.Priority = 'medium';
    }
  }
}
```

**Scenario 2:**
When a lead is created with LeadSource as Web, set rating as cold; otherwise, set it as hot.

```apex
trigger LeadRating on Lead (before insert) {
  for (Lead ld : Trigger.new) {
    if (ld.LeadSource == 'web') {
      ld.Rating = 'cold';
    } else {
      ld.Rating = 'hot';
    }
  }
}
```

**Scenario 3:**
Automatically create an associated contact when a new account record is created.

```apex
trigger AccountAfter on Account (after insert) {
  List<Contact> cons = new List<Contact>();
  for (Account acc : Trigger.new) {
    Contact c = new Contact();
    c.LastName = acc.Name;
    c.Phone = acc.Phone;
    c.Email = acc.Email;
    cons.add(c);
  }
  insert cons;
}


```

