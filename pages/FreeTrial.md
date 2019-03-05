# Free Trial page
This document describes the `Free Trial` CTA form.
* URL: https://www.gondolatest.com/en/free-trial
* Wireframe: [/wireframes/free-trial-page.svg](../wireframes/free-trial-page.svg)

## Fields
Check out the fields displayed on the wireframe

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
  Gondola Team @ LogiGear
  ```

> Contact designer for the beautified version of this email.