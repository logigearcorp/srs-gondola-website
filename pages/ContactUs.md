# Contact Us page
This document describes the `Contact Us` CTA form.
* URL: https://www.gondolatest.com/en/contact-us
* Wireframe: [/wireframes/contact-us-page.svg](../wireframes/contact-us-page.svg)

## Fields
Check out the fields displayed on the wireframe.

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