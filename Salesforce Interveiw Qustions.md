# Salesforce Questions 

### Salesforce Admin Basics

1.  What is cloud Computing?
2.  What is Paas, Saas, Iaas?
3.  What is Sandbox and the Type of Sandbox in Salesforce?
4.  What is Object in Salesforce?
5.  What are the different types of object relations in Salesforce.
6.  What is a Master--Detail relationship in Salesforce?
7.  What is a junction object in Salesforce?
8.  How many LR(lookup relationship) fields can be created in an object?
9.  What is a Roll-up Summary field
10. How many way to create What is a Roll-up Summary field
11. What is field dependency
12. What is the difference between role and profile
13. What are Permission sets?
14. What is use of muting permission set in permission set group
15. How many ways we can share a record?
16. What are Audit Fields in Salesforce?
17. What is an Audit trail?
18. What is a Queue in Salesforce?
19. What is a Public Group
20. Difference between static and dynamic dashboards in Salesforce?
21. What are the different types of reports available in Salesforce?
22. What is Report Type?
23. What are WhoId and WhatId in activities?
24. What is a bucket field in reports?
25. Way to clean data in Salesforce
26. Differences between Import wizard and Data loader
27. What is "Data Skew" in Salesforce
28. What is cascade deletion?
29. What is a Flow?
30. Types of flows in Salesforce
31. Name a few global variables which are used in formula and validation rules.
32. Is there any special permission available to edit read only fields. Please explain
33. What are the differences between Object-specific action and global actions?
34. Mention one impact point to check before deleting a role from the org.
35. Let's say I create two accounts a1 and a2. Now I make a2 as the parent of a1. Now what will happen if I try to make a1 parent of a2
36. How do you pass the current record id to a screen flow? Also is it possible to send the entire record?
37. How do you check your org is in which release
38. What is a big object? Give an example of a standard big object
39. Is it possible to use formula field in roll up summary calculation which is referring to another object?
40. Suppose there is a custom field which has a default value but not added to the page layout. Now, if you clone a record from the UI, what would be the value of the field in the new record?
41. What is the consideration while deleting an approval process?
42. What happens during Lead merging?
43. What is Apex Hammer?
44. How do you convert 15 digit record Id to 18 digit Id in formula and validation rule?
45. Is it possible to hard delete records using data loader?
46. Is it possible to show validation errors in screen flow?
47. You have created a custom object. While creating a report on the object, you are not getting the option to select the object in the report builder. What could be the issue?
48. What are the possible statuses of a permission set group?
49. How can we enable email approval response? Mention a few response keywords which will approve/reject the request
50. You are not getting an option to create list custom settings. Which setting needs to be enabled?
51. Once a lead is converted it is not visible anymore in the UI. Is there any permission available to view converted leads?
52. You are trying to convert a master detail relationship field to lookup relationship. But you are not able to see the change field type button. What could be the reason?
53. One of the users in your org is not able to create campaigns. You checked the profile/ permission sets and ensured that he has access to create campaigns. What could be the reason?
54. What happens when you try to delete a public group?
55. What happens when you try to delete a queue?


### Salesforce Dev 

1.  What is Sandbox and the Type of Sandbox in Salesforce?
2.  What is Cloud Computing?
3.  What is Iaas?
4.  What is PaaS?
5.  What is Saas?
6.  Type of Object Relationship in Salesforce?
7.  What is Junction Object in Salesforce?
8.  What is the difference between Role and Profiles?
9.  How many way we have in Salesforce for Sharing?
10. What are Sharing Rules?
11. What is Manual Sharing?
12. What is Apex Sharing?
13. Type of Flow in Salesforce?
14. When to use Flow vs Apex?
15. Best practices for Salesforce Flow?
16. What is Apex? and when to use Apex over Flow?
17. What are Apex Best practices in Salesforce?
18. What is Apex Trigger? and When we should use Apex Trigger?
19. What is Apex Trigger Handler pattern?
20. What is Apex Trigger Framework? What are different Trigger Framework are available in Salesforce?
21. What is Async Apex in Salesforce? How many way we have for Async processing?
22. What is Batch job in Salesforce?
23. What is difference between Stateful and Stateless batch job?
24. What is mixed DML?
25. What is Lightning Data Service?
26. How to do communication between Lightning web component?
27. How to call Apex class in Lightning web component and how many way we have and when to use which option?
28. What are the basic difference between Application Event and Component Event in Aura component?
29. What is lightning messaging service?
30. What is lazy loading in LWC and how do lazy loading in LWC?
31. What are Design Attributes in Lightning Web Components?
32. What is web services?
33. What is the difference between SOAP and REST?
34. What is the difference between Enterprise WSDL and Partner WSDL?
35. Explain about Integration Patterns?


### Salesforce Intergration

1.  What is Integration?
2.  What is webservices?
3.  Difference between JSON Vs XML ?
4.  What is REST API ?
5.  What is SOAP API ?
6.  What is difference between SOAP and REST?
7.  What all Integration option are available in Salesforce?
8.  What is WSDL?
9.  What is SoapUI?
10. What is difference between Enterprise WSDL and Partner WSDL?
11. What is an Integration Patterns?
12. Different type of Integration patterns available in Salesforce?
13. What is remote site settings?
14. What is a Connected App?
15. What is OAuth?
16. What are different OAuth2.0 Authorization flows are available in Salesforce?
17. What is JWT flow in Salesforce?
18. What is web service flow in Salesforce?
19. What is Named Credentials and what is the use of it?
20. **What is OpenID Connect**?
21. **Difference between OpenID and OAuth**?
22. What is Streaming API? Explain the different mechanism of Steaming API?
23. What is Change Data Capture?
24. What is Tooling API? Provide one example when you used it.
25. What is Salesforce Connect?
26. What are REST API Composite Resources


### Triggers

1.  What is Trigger in Salesforce?
2.  What are the two types of triggers in Salesforce?
3.  What is the use of trigger class in Salesforce?
4.  What are different events available in Triggers?
5.  When we should use trigger or automation?
6.  Best practice and consideration for Trigger?
7.  How many times trigger execute on an Upsert event
8.  How many times trigger execute on an Merge event
9.  Order of execution for Trigger
10. When you will choose before event and when you will chose after event?
11. What is the different between Trigger.New and Trigger.newMap?
12. When we should use Trigger.Old
13. How to void recursion in Trigger.
14. How make callout from Trigger?
15. Can we call a batch job from Trigger?
16. What is Trigger Handler pattern?
17. Have you used any trigger framework in Salesforce?
18. **Difference between Validation rules and Triggers?**


## Lightning 

1.  How can we extend any component in aura framework?
2.  How can you call one JS controller method from another JS controller method in aura?
3.  How do you pass value to the JS controller while using hyperlink?
4.  What are the steps to add a lightning component in a vf page?
5.  How do you de-activate the paste functionality in lightning input?
6.  How to get the current user name and current user profile name in aura component without using apex?
7.  Explain data binding in aura
8.  Why do we use @AuraEnabled annotation?
9.  Is it possible to use the value of another attribute or any custom label as the default value of one attribute in aura component instead of using hardcode?
10. How do we restrict an aura component to be used in the record pages of only for particular Sobjects?

