# Group-Zero-Code-Institute

**Group-Zero-Code-Institute** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Project Overview
* This project is about checking whether passwords meet basic security rules. This will enable the business to protect its data and mitigate against cyberattacks, ensures that it is compliant with legislative considerations such as the Data Protection Act and reduce risks associated with data breaches. This project will provide a step-by-step approach on how to follow a clear set of rules to ensure personal and professional safety.
* Milestone Project for Predictive Analytics Specialisation at Code Institute: Predicting Password Security
* Scenario:

Password Requirements Scenario:  
Check if passwords meet basic security rules (minimum 8 characters, contains numbers).    
Data:  passwords = ["hello123", "cat", "secure2024", "password"]   
Tasks:  
a) Check each password's length. 
b) Create a list of passwords that are 8 or more characters long. 
c) come up with your own rules - no restrictions - think like your own application you are developing  

## Password Requirements
* The business requirements include the checking of all passwords to ensure that they meet the condition of 8 characters or including numbers.

## Hypothesis and how to validate

* Hypothesis: Most user-created passwords fail to meet minimal length and numeric requirements.
* Validation: Run the program and compare how many passwords pass or fail the checks.

Validation:
Run the Python script to test each password.
Passwords meeting both criteria are collected in a list of accepted passwords.

## Project Plan
Milestone Project for Predictive Analytics Specialisation at Code Institute: Predicting Password Security.

1. **Collect Data:** Create a small list of example passwords.
   We used the following passwords to test our program:
   (Enter the passwords).
3. **Define Rules:** Implement two functions — one for length, one for number presence.
   We use the Python length function to check the password length.
   We are going to check the passsword if it contains a number or a numerial number within the 8 character length limit. 
   (Show the command from python - decide whether to include or not.) 
5. **Evaluate Passwords:** Loop through all passwords, apply both checks.
   We loop through the password list and checked the above Two conditions - length and number.
   We used the list data structure to store password list.
7. **Store Results:** Append successful passwords to a new list.
   The passwords which satisfy the above requirement are added to a new list which can be printed out. 
9. **Print Results:** Display which passwords passed validation.
   Passwords that have met all the conditions will be printed out.

## Analysis techniques used

Predictive Analytics Specialisation: Predicting Password Security.
- **Iteration and Condition Checking:** Loops through each password and validates conditions.  
- **Functional Approach:** Uses small, reusable functions for clarity and testing.  
- **Python Built-ins:** Utilizes `any()`, `isdigit()`, and `len()` to simplify logic.  

### Limitations
The current version does not check for uppercase, lowercase, or special characters — future iterations may include these.

Generative AI  was used to explore ideas around risk to businesses and password implementation. We also looked at legistlation and data protection (GDPR) regarding password protection. 
During the password-validation project, we used generative-AI tools to brainstorm secure and user-friendly design options. In the ideation phase, we prompted AI to propose multiple validation strategies and evaluate their pros and cons.

## Ethical considerations
* No real user data was used. The passwords are purely synthetic examples to avoid privacy issues.

## Development Roadmap
* Add integration with user input for live password validation.
* Incorporate regex for advanced password strength scoring.

## Deployment
ï»¿"passwords = [""hello123"", ""cat"", ""secure2024"", ""password""]  accepted = [ ] not_accepted =[ ]  for x in passwords:     if not len(x) < 8:         if (any(char.isdigit() for char in x)):             accepted.append(x)         else:             not_accepted.append(x)     else:         not_accepted.append(x)          print(f""{accepted} accepted passwords"") print(f""{not_accepted} not accepted passwords"")"

"passwords = [""hello123"", ""cat"", ""secure2024"", ""password""]  def password_leng(password):     return len(password) >= 8  def password_has_number(password):     return any(char.isdigit() for char in password)  result = {}  for password in passwords:     result[password] = {         ""length_ok"": password_leng(password),         ""has_number"": password_has_number(password)     }  print(result)     "

"passwords = [""hello123"", ""cat"", ""secure2024"", ""password""]  pass_pass = [] pass_fail=[] for password in passwords:         if len(password) >= 8:                  pass_pass.append(password)          else:                  pass_fail.append(password)  print(pass_pass)   or   passwords = [""hello123"", ""cat"", ""secure2024"", ""password""]  pass_check = {}   for password in passwords:   if len(password) >= 8:                  pass_check.append(password:True)          else:                  pass_check.append(password:False)   print (pass_check(""hello123""))"

ï»¿"passwords = [""hello123"", ""cat"", ""secure2024"", ""password""]   â€ƒdef password_check(password): â€ƒâ€ƒif password.lengh()>=8: â€ƒâ€ƒâ€ƒreturn: True â€ƒâ€ƒâ€ƒelse: False    password_check(passwords[1])  password_check(passwords[2])"

### Acknwowledgements

- Ace
- Baba
- Raphael
- Vish
- Volodymr
- Unniki
- Anisa
- Jasbinder
