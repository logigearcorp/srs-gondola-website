# Newsletter Subscription
This document describes the `Newsletter Subscription` CTA form.

## Fields
Data fields on the form that users must fill in.

Field | Mandatory | Validation | Example
------|-----------|------------|--------
Work email | Y | Valid email address | john.doe@supercoolcorp.com
Opt-in | Y | default: unchecked | Display text: "I would like to subscribe to updates from LogiGear". Only when users check this checkbox, we enable the Subscribe button
Question-mark hover-button | N/a | N/a | Display this text when users hover on the question mark: "You will occasionally receive newsletters about product updates, testing best practices and events from us"

## Position
* Subscription box on Home page at www.gondolatest.com


## Functionality
* Must prevent spamming by reCAPTCHA v3
* When the user submit the form, send an email to support@gondolatest.com.

  ```
  Title: New Newsletter Subscription
  
  Content:
  Hi Sales/Support, 
  The following prospect has submitted a request for Newsletter.
  [All data collected]
  This email address has been added to Pardot.
  Thanks.
  Best regards,
  Automatic sender
  ```

* Add this email address to Pardot under the list `Gondola-Newsletter`
* Send this email to the registered email address:

  ```
  Title: Thank You for Subscribing to our Newsletter
  
  Content:
  Hi [Name], 
  We have received your subscription request. Stay tuned for newsletters from us.
  Thanks.
  Best regards,
  Gondola Team
  ```

> Contact designer for the beautified version of this email.
