# Pricing page
* URL: https://www.gondolatest.com/en/pricing
* Wireframe: [/wireframes/pricing-page.svg](../wireframes/pricing-page.svg)

## Behaviors
* Display the UI controls as described in the wireframe
* Pick a license type: radio button
* Pick a License Server type: radio button
* Pick how many licenses: number of licenses must be greater than zero
* When users hover on the question-mark next to Node-Locked Licenses > Display this tooltip: "Node-Locked licenses are tied to specific machines but, within some constraints, may be reassigned"
* When users hover on the question-mark next to Floating Licenses > Display this tooltip: "Under a Floating license, Gondola may be used on one local network by different machines and devices at the same time up to the number of floating seats licensed. If a license is available, the License Server allows Gondola applications to occupy it. When a user finishes using Gondola, the license is reclaimed by the License Server and made available to other users."
* When users hover on the question-mark next to "Floating Test Runners" > Display this tooltip: "Floating Test Runners are used for test execution only. Typically, you can use these licenses on virtual machines ito parallel your test execution. This is a floating license which can be shared concurrently by multiple machines and/or devices."
* Pick automation platforms: users can multi select, default: all checkboxes are checked
* Users must tick the 2 "I accept..." checkboxes to submit
* Must prevent spamming using reCAPTCHA v3
* When the user submits the form, send an email to support@gondolatest.com.

  ```
  Title: [ATTENTION] QUOTING REQUEST
  
  Content:
  Hi Sales/Support, 
  The following prospect has requested a quoting for Gondola.
  [All data collected]
  This email address has been added to Pardot.
  Thanks.
  Best regards,
  Automatic sender
  ```

* Add this email address to Pardot under the list `Gondola-SQL`
* Send this email to the registered email address: 
  
  ```
  Title: Thank You for Requesting Gondola Quotes
  
  Content:
  Hi [Name], 
  We have received your request to quote Gondola. Our Sales team will respond to you as soon as possible. Stay tuned.
  Thanks.
  Best regards,
  Gondola Team
  ```

> Contact designer for the beautified version of this email.