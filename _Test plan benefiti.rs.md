  
**Test plan \- [Benefiti.rs](http://Benefit.rs)**

Author: Marko Kerac  
Date:22.5.2025

**Table of Contents**

1. **Introduction \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 2**  
   **1.1 Objectives**  
   **1.2 Team members**  
2. **Scope of testing \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 2**  
3. **Risk assessment\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 3**  
4. **Test approach  \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 3**  
5. **Resources \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 3**  
6. **Test environment   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 3**  
7. **Criteria\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 4**  
8. **Schedule\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_page 4**

   

**1\. Introduction**

This Test Plan is designed to describe the scope, approach, resources, and schedule of all testing activities for the [Benefiti.rs](http://Benefiti.rs) website.  
This plan identifies the items to be tested, the features to be tested, the types of testing that will be performed, the persons responsible for testing, the resources and schedule required to complete testing, and the risks related to the plan.  
	  
**1.1 Objectives**

The **Benefiti.rs** application is an SaaS platform designed for companies that want to offer their employees personalised benefits within a defined budget. It helps employers to create attractive benefit packages while giving employees the freedom to choose the benefits that suit them best.

**1.2 Team members**

* Marko Kerac- QA   
* Anastasia Engelhardt-Mentor  
* Tamara Cvetkovic-Mentor

**2\. Scope of testing**

This test plan covers one of the key functionalities: **Benefit group creation and management**.

The following functionalities will be tested:

1. Creating a new benefit group  
2. Adding all relevant information and photos to the group  
3. Adding new benefits to the group  
4. Editing or deleting benefits within the group  
5. Editing or deleting the group itself

   

**3\. Risk assessment**  
The following risks have been identified, and the appropriate solutions are described to reduce their impact on the project:

| nr. | Risk | Impact | Trigger | Solution |
| :---: | :---: | :---: | :---: | :---: |
| 1\. | Incomplete requirements could lead to incorrect assumptions in test design. | High | Missing or vague details in requirement specifications. Misalignment between development, QA, and product teams regarding requirements | Ensure QA participation in all requirement-related meetings Encourage communication and clarification with stakeholders  |
| 2\. | Insufficient time for testing | High | Development is delayed, reducing the time available for testing | Define and communicate clear testing timelines and priorities with stakeholders”  |
|  |  |  |  |  |

**4\. Test approach**

1. This test plan will follow an agile approach with weekly iterations  
2. Testing will be executed manually as our project time is short  
3. The tests will focus on the key functionalities and user interface, from the perspective of employees and HR users.  
4. Due to the lack of SRS documentation and the team's inexperience with the web application, the team will initially rely on exploratory testing to uncover unexpected behaviours and document actual functionalities..  
5. Testing types that will be included:   
   1. Functional testing  
   2. UI/UX verification  
   3. Field validation   
   4. Edge case testing

   

**5\. Resources**

* PC/Laptop \- Windows 10 or newer  
* Internet connection  
* Demo account at: [https://demo.benefiti.rs/\#/](https://demo.benefiti.rs/#/)  
* Project management tool: Jira  
* Test management software: Qase

**6\. Test environment**

Testing will take place on a demo version of a live web application, on the following address:[https://demo.benefiti.rs/\#/](https://demo.benefiti.rs/#/)

**7\. Criteria**

* **Entry**  
  * The application is available

  * The demo account is created and verified

  * Functionalities have been implemented

* **Exit**  
  * Test cases are executed

  * The bugs have been recorded and reported

  * Test plan completed and delivered

**8\. Schedule**

* Creation of the Test Plan 22.5.2025   
* Manual testing 22.5.-23.5.2025  
* Bug report creation 22.5-23.5.2025  
* Test plan completion and submitting 23.5-24.5.2025  
    
  