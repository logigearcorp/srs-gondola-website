# Free Trial page
This document describes the `Free Trial` CTA form.
* URL: https://www.gondolatest.com/en/free-trial
* Wireframe: [/wireframes/free-trial-page.svg](../wireframes/free-trial-page.svg)

## Fields
Data fields on the form are listed below.

Field | Mandatory | Validation | Example
------|-----------|------------|--------
Name | Y | Length < 100 chars | John Doe
Work email | Y | Valid email address | john.doe@supercoolcorp.com
Company | Y | Length < 100 chars | Super Cool Corp
Phone | **Y** | N/a | 650-111-8989
Country | N | Pick among a list | United States
Testing needs | Y | Pick among a list | Web Testing & Mobile Testing
Business title | Y | N/a | Senior QA Engineer
Partner referral | N | Pick from a list | SEPTech
I accept EULA & Privacy Policy | Y | Checkbox | N/a

## Functionality
* Must repvent spamming using reCAPTCHA v3
* When the user submits the form, send an email to support@gondolatest.com.

  ```
  Title: [ATTENTION] FREE TRIAL REQUEST
  
  Content:
  Hi Sales/Support, 
  The following prospect has submitted a trial request for Gondola.
  [All data collected]
  This email address has been added to Pardot.
  Thanks.
  Best regards,
  Automatic sender
  ```

* Add this email address to Pardot under the list `Gondola-SQL`
* Send this email to the registered email address: 
  
  ```
  Title: Thank You for Requesting Gondola Free-Trial
  
  Content:
  Hi [Name], 
  We have received your request to try out Gondola for free. Our Customer Support team will respond to you as soon as possible. Stay tuned.
  Thanks.
  Best regards,
  Gondola Team
  ```

> Contact designer for the beautified version of this email.