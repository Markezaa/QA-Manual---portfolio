**Bug Report 2\. \- Benefiti email**

**Title/Summary:** In the “Add Employee/Dodaj zaposlenog” functionality, an Invalid email address **(.con)** is accepted when registering a new user.

**Description:** When registering a new user in the system, an invalid email format (according to ICANN), such as “abc@example.**con,**” is accepted in the email field.

**Environment:** Desktop, Google Chrome 136.0.7103.114 (Official Build)

**Precondition:** Log in as HR.

**Steps to Reproduce:** 

1. Go to [https://demo.benefiti.rs/\#/](https://demo.benefiti.rs/#/).  
2. .  
3. In the left navbar, click on “Zaposleni (or Employees, depending on language settings).  
4. Click on the big blue button “Dodaj zaposlenog” or “ Add Employee”, at the top right corner of the page.  
5. Fill out mandatory fields: name, surname and location.  
6.  Input invalid email (email ending with **.con**)  
7. Click on the blue “Dodaj”/”Add” button at the bottom of the page.

**Expected Results:** The User has not been added, and an error message has been shown, implying that the email address is invalid.

**Actual Results:** The Process is completed, and the user has been added successfully to the system.

**Severity: High**

**Priority: High**

