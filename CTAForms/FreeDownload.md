# Free Download
This document describes the `Free Download` CTA form.

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

## Position
* URL: www.gondolatest.com/free-download
* `Free Download` button floating on the main Nav-bar that appears on every page

## Functionality
* Must have CAPTCHA
* When the user submit the form, send an email to support@gondolatest.com.

  ```
  Title: [ATTENTION] FREE DOWNLOAD REQUEST
  
  Content:
  Hi Sales/Support, 
  The following prospect has submitted a request for Gondola Essential.
  [All data collected]
  This email address has been added to Pardot.
  Thanks.
  Best regards,
  Automatic sender
  ```

* Add this email address to Pardot under the list `Gondola-SQL`
* Send this email to the registered email address: 
  
  ```
  Title: Thank You for Requesting Gondola Essential
  
  Content:
  Hi [Name], 
  We have received your request to download Gondola Essential for free. Our Customer Support team will respond to you as soon as possible. Stay tuned.
  Thanks.
  Best regards,
  Gondola Team
  ```

> Contact designer for the beautified version of this email.