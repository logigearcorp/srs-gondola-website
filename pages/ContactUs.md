# Contact Us page
This document describes the `Contact Us` CTA form.
* URL: https://www.gondolatest.com/en/contact-us
* Wireframe: [/wireframes/contact-us-page.svg](../wireframes/contact-us-page.svg)

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

## Functionality
* Must prevent spamming by reCAPTCHA v3
* When the user submits the form, send an email to support@gondolatest.com.

  ```
  Title: Somebody Contacted Us
  
  Content:
  Hi Sales/Support, 
  The following prospect has sent us a message.
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
  Title: Thank You for Contacting LogiGear
  
  Content:
  Hi [Name], 
  We have received your message below.
  [Message]  
  Our Customer Support team will respond to you as soon as possible. Stay tuned.
  Thanks.
  Best regards,
  Gondola Team @ LogiGear
  ```

> Contact designer for the beautified version of this email.