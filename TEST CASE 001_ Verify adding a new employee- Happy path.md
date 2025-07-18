**TEST CASE 001**: Verify adding a new employee with valid input values  
**Priority:** High  
**Preconditions:**   
The user is logged in with an HR account.

| Step | Test Steps | Test Data | Expected Results |
| :---: | :---: | :---: | :---: |
| 1\. | Click on the Employee section from the sidebar. | / | The employee section is displayed. |
| 2\. | Click on the "+ Add Employee" button. | / | User is redirected to the “Add Employee” page. |
| 3\. | Fill in the mandatory Name field: |   Nikola | The "Name" field displays "Nikola". The avatar field shows a circle with "N" inside it. |
| 4\. | Fill in the mandatory Last Name field: |  Jokic | The "Last Name" field displays "Jokic". The avatar field shows a circle with "NJ" inside it. |
| 5\. | Fill in the mandatory Email field: | nikola.jokic@gmail.com | The “Email ” field displays  “[nikola.jokic@gmail.com](mailto:nikola.jokic@gmail.com)” email address |
| 6\. | Click on the “Locations” field, and select a location from the drop-down menu  | Aranđelovac | The “Location” field displays “Adanđelovac” |
| 7\. | Click on the “Tier” field, and select a tier level from the drop-down menu | 300-tokena | The “Tier” field displays “300-tokena” |
| 8\. | Click on the “Add” button | / | The employee list and the bright green pop-up window “ User successfully added” are displayed. |
| 9\. | Verify that the employee with matching credentials is in the list. |  | The user with these credentials is in the employee list: Nikola Jokic, 300 tokena, [nikola.jokic@gmail.com](mailto:nikola.jokic@gmail.com)  |

