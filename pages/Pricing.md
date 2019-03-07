# Pricing page
* URL: https://www.gondolatest.com/en/pricing
* Wireframe: [/wireframes/pricing-page.svg](../wireframes/pricing-page.svg)

## Behaviors
* Display the UI controls as described in the wireframe

* **Pick a license type**: select either one of the options
    * When users hover on the question mark next to this field, display this tooltip: "Perpetual licenses grant you sole ownership of the software that lasts for 99 years. Besides this one-time payment option, you can choose to pay monthly or annually (SaaS)."

* **Pick a License Server type**: select either one of the options
    * When users hover on the question mark next to this field, display this tooltip: "You can either choose to host Gondola License Server on your own or let us host it for you. For the cloud option, you must have constant internet connection to perform heartbeat license validations."

* **Pick how many licenses**
    * The number of licenses must be greater than zero and less than 1,000
    * Numeric characters only
    * No decimal
    * When users hover on the question-mark next to "Node-Locked Licenses", display this tooltip: "Node-Locked licenses are tied to specific machines but, within some constraints, may be reassigned to other machines."
    * When users hover on the question-mark next to "Floating Licenses", display this tooltip: "Under a Floating license, Gondola may be used on one local network by different machines and devices at the same time up to the number of floating seats licensed. If a license is available, the License Server allows Gondola applications to occupy it. When a user finishes using Gondola, the license is reclaimed by the License Server and made available to other users."
    * When users hover on the question-mark next to "Floating Test Runners", display this tooltip: "Floating Test Runners are used for test execution only. Typically, you can use these licenses on virtual machines to parallel your test execution. This is a floating license which can be shared concurrently by multiple machines and/or devices."

* **Frequently Asked Questions:** display a collapsible accordion under this title of this section
    * How much does Gondola cost? --> "We offer flexible pricing that fits your organization's specific needs. Please submit this form or call us at +1 (800) 322-0333 (USA) or +81 50 3699 4492 (Japan) to get a quote."

    * How do I purchase Gondola? --> "Please submit this form or call us at +1 (800) 322-0333 (USA) or +81 50 3699 4492 (Japan) to get a quote. Our sales team will contact you shortly."

    * What is the difference between Node-Locked and Floating licenses? --> "A Node-Locked license is tied to a specific machine so you got less flexibility while Floating licenses can be shared among your team members."

    * Is it possible to upgrade Node-Locked to Floating? --> "Yes. You can convert any number of Node-Locked licenses to Floating licenses with a certain fee and conditions."

    * What is License Server? --> "Gondola License Server (LS) is a free software used to manage your licenses. LS must be installed in a physical machine before you can start using Gondola. Normally, only one LS is needed in your network. Once you pay the license fees, you'll receive a license key which specifies how many and what types of licenses you can use. In order to obtain this license key, you will need to provide us the host name or IP address of the machine that will host the LS."

* **Pick automation platforms**: 
    * Users can multi select
    * Default: all checkboxes are checked

* Users must tick the 2 "I accept..." checkboxes to submit the form

* Must prevent spamming using reCAPTCHA v3

* When the user submits the form, send an email to support@gondolatest.com.

  ```
  Title: [ATTENTION] QUOTING REQUEST
  
  Content:
  Hi Sales/Support, 
  The following prospect has requested a quote for Gondola.
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
  We have received your request for a quote of Gondola. Our Sales team will respond to you as soon as possible. Stay tuned.
  Thanks.
  Best regards,
  Gondola Team
  ```

> Contact designer for the beautified version of this email.