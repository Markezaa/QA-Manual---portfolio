**TEST CASE 002**: Verify adding a new employee with an empty mandatory email field is not possible, and the error message is displayed.  
**Priority:** High  
**Preconditions:**   
The user is logged in with an HR account.

| Step | Test Steps | Test Data | Expected Results |
| :---: | :---: | :---: | :---: |
| 1\. | Click on the Employee section from the sidebar. | / | The employee section is displayed. |
| 2\. | Click on the "+ Add Employee" button. | / | User is redirected to the “Add Employee” page. |
| 3\. | Fill in the Name field: | “Dragan” | The "Name" field displays "Dragan". The avatar field shows a circle with "D" inside it. |
| 4\. | Fill in the Last Name field: | “Dragic” | The "Last Name" field displays "Dragic". The avatar field shows a circle with "DD" inside it. |
| 5\. | Click on “Add” | / | The system does not add a new user, and red text saying “Mandatory field” is displayed above the email field |
| 6\. | Fill in the Email field: | dragan.dragic@gmail.com | “[dragan.dragic@gmail.com](mailto:dragan.dragic@gmail.com)” is displayed in the Email field, and the error message is not shown; instead, the bright green pop-up window “ User successfully added” is shown |

