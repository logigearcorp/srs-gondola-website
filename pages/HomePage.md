# Home Page
* URL: https://www.gondolatest.com
* Wireframe: [/wireframes/home-page.svg](../wireframes/home-page.svg)

## Behaviors
* Display the UI controls as described in the wireframe
* When users click on Free Trial > Open the `Free Trial` page
* When users click on Learn More > Open the `Features` page
* When users click "Docs" menu item > Open [https://docs.gondolatest.com](https://docs.gondolatest.com)
* Please contact Graphics Designer for icons
* "Write Easy to Understand Automation Scripts" section
    * Users hover on the _left_ image > Shows "Behavior-Driven Development (BDD)" box on top of the image
    * Users hover on the _right_ image > Shows "Keyword-Driven Testing (KDT)" box on top of the image
* When users click "Contact Us" button > Open the `Contact Us` page

## Newsletter Subscription Form
Below is the description of the `Newsletter Subscription` CTA form

### Fields
Data fields on the form that users must fill in.

Field | Mandatory | Validation | Example
------|-----------|------------|--------
Work email | Y | Valid email address | john.doe@supercoolcorp.com
Opt-in | Y | default: unchecked | Display text: "I would like to subscribe to updates from LogiGear". Only when users check this checkbox, we enable the Subscribe button
Question-mark hover-button | N/a | N/a | Display this text when users hover on the question mark: "You will occasionally receive newsletters about product updates, testing best practices and events from us"

### Functionality
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
