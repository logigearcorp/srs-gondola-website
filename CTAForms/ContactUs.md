# Contact Us
This document describes the `Contact Us` CTA form.

## Fields
Data fields on the form are listed below.

Field | Mandatory | Validation | Example
------|-----------|------------|--------
Name | Y | Length < 100 chars | John Doe
Work email | Y | Valid email address | john.doe@supercoolcorp.com
Company | Y | Length < 100 chars | Super Cool Corp
Phone | N | N/a | 650-111-8989
Country | N | Pick among a list | United States
Business title | **N** | N/a | Senior QA Engineer
Message | Y | N/a | I want to buy 10 licenses

## Position
* URL: www.gondolatest.com/contact-us
* `Contact Us` menu item on the main Nav-bar

## Functionality
* Must have CAPTCHA
* When the user submit the form, send an email to support@gondolatest.com.

  ```
  Title: Somebody Contacted Us
  
  Content:
  Hi Sales/Support, 
  The following prospect has sent a message.
  [All data collected]
  Please respond as soon as possible. 
  This email address has been added to Pardot.
  Thanks.
  Best regards,
  Automatic sender
  ```

* Add this email address to Pardot under the list `Gondola-MQL`
* Send this email to the registered email address: 
  
  ```
  Title: Thank You for Contacting Us
  
  Content:
  Hi [Name], 
  We have received your message below.
  [Message]  
  Our Customer Support team will respond to you as soon as possible. Stay tuned.
  Thanks.
  Best regards,
  Gondola Team
  ```

> Contact designer for the beautified version of this email.