# Test Cases for Login Page

## TC-01: Login with valid data
- **Test priority:** High
- **Summury:** Login with valid data
- **Precondition:**  
*Username:* tomsmith  
*Password:* SuperSecretPassword!  
*Entry point:* https://the-internet.herokuapp.com/login  
- **Steps:**  
    1. Insert *Username* at the field "Username"
    2. Insert *Password* at the field "Password"
    3. Push at the buttom "Login"
- **Expected result:** User redirect at the Secure Area page

---

## TC-02: Login with invalid data
- **Test priority:** High
- **Summury:** Login with invalid *Username*
- **Precondition:**  
*Password:* SuperSecretPassword!  
*Entry point:* https://the-internet.herokuapp.com/login 
- **Steps:**  
    1. Insert *Username* (ex. "tom") at the field "Username"
    2. Insert *Password* at the field "Password"
    3. Push at the buttom "Login"
- **Expected result:** Resived message "Your username is invalid!"

---

## TC-03: Login with invalid data
- **Test priority:** High
- **Summury:** Logine with invalid data *Password* 
- **Precondition:**  
*Username:* tomsmith  
*Entry point:* https://the-internet.herokuapp.com/login
- **Steps:**  
    1. Insert *Username* at the field "Username"
    2. Insert any *Password* (ex. "Password") at the field "Password"
    3. Push at the buttom "Login"
- **Expected result:** Resived message "Your password is invalid!"

---

## TC-04: Check function "Login" without data
- **Test priority:** Mid
- **Summury:** checking the system to provide feedback on the need to enter data into fields
- **Precondition:**  
The fields "Username" and "Password" are empty  
*Entry point:* https://the-internet.herokuapp.com/login
- **Steps:**  
    1. Push at the buttom "Login"
- **Expected result:** Resived message "Your username is invalid!"

---

## TC-05: Checking system on SQL injection
- **Test priority:** High
- **Summury:** checking that the system does not provide data from the database
- **Precondition:**  
*Entry point:* https://the-internet.herokuapp.com/login
- **Steps:**  
    1. Insert *' OR '1'='1 --* at the field "Username"
    2. Insert any *Password* (ex. "Password") at the field "Password"
    3. Push at the buttom "Login"
- **Expected result:** Resived message "Your username is invalid!"