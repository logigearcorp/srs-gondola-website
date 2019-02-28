# Introduction
This repository contains the Software Requirement Specification document and related artifacts that support the development of the Gondola website.
* Domain: www.gondolatest.com
* SRS document: www.github.com/thucldnguyen/srs-gondola-website
* Current version: v1.0.1
* Source code repository: [TBD]

# About Gondola
Gondola is a freemium test automation framework that makes Continuous Delivery a reality. Gondola is tester-friendly while powerful for SDET and developers alike.

# Sitemap
The Gondola website's frontend must follow the below structure.
~~~~
Home (Why Gondola?)
    +-- Features
    +-- Pricing
    +-- Resources
        +-- Docs
        +-- Tutorials        
    +-- Blog    
    +-- About Us
    +-- Free Trial (CTA)
    +-- Contact Us (CTA)
    +-- EULA
    +-- Privacy Policy
~~~~

# Non-functional Requirements
The Gondola website must satisfy the below non-functional requirements.
* Lightning FAST (response time <= 4 seconds)
* Responsive design on Desktop, Mobile and Tablet
* Beautifully designed look & feel on the frontend
* Different color theme than www.pombuilder.com, www.logigear.com and www.testarchiect.com

# Functional Requirements
The Gondola website must satisfy the below functional requirements.

## Standard CMS Features
Backend users must be able to CRUD contents displayed on the frontend. Frontend users must be able to read and interact with the managed contents. Objects we want to manage:
* Page management
* Post management
* User management

> NOTE: Must support Markdown when editing articles.

## Wireframes
Please check out the images inside the `./wireframes` folder.

## HTTPS Support
This website must support `https` protocol using **Letsencrypt**.

## Frontend Localization
Visitors must be able to switch between multiple languages following the below priority.

Priority | Language
---------|---------
1 | Japanese 
2 | English 

> NOTE: This requirement only applies to the frontend. 

More detailed requirements:
* Each content object (article, page, section, form, etc.) must have multiple versions. Each version corresponds to a language.
* Backend users must be able to edit each language version of the same article separately.
* When frontend users switch languages, all content objects must be reloaded accordingly.

## Cookies Agreement Notice
Visitors must accept the Cookies Agreement in order to proceed. When frontend users visit www.gondolatest.com for the first time, they will see this cookies usage notification.  After they accept the terms, we no longer ask for their permission. We'll use Cookies to improve UX as described below.

## UX Improvements Using Cookies
When frontend users fill a CTA form and submit their personal data, we'll store some of that data such as 'job title' in Cookies to tailor our website later [TBD].

## Pardot Integration
All registered email addresses must be added to Pardot's database. For credentials of our corporate Pardot account, please contact _Thuc Nguyen_ (thuc.nguyen@logigear.com).

## Blog Page
This section must satisfy the following requirements. 
* Frontend users must be able to read posts
* Posts must be paginated
* Visitors must be able to share articles on social media (Facebook and Twitter)

## CTA forms
We display the following CTA forms on our website.
* [Newsletter Subscription Form](./CTAForms/NewsletterSubscription.md): subscribe to our newsletters. 
* [Free Download Form](./CTAForms/FreeDownload.md): download the Gondola Essential package for free. 
* [Contact Us](./CTAForms/ContactUs.md): send an email to our Customer Support. 

All prospects will be able to receive email notifications from us.  

> NOTE: 
> * Exact position, visual design, and functionality of each CTA form will be described in `./CTAForms`.
> * This website's email notification feature has nothing to do with email marketing campaigns in Pardot.

## Analytics
* Google Analytics and basic SEO tools provided by WordPress must be supported.
* Yoast SEO plugin (free) must be preinstalled

# Out-scope
The following functions are not necessary in the current version of the website.
* No need for search function on the frontend
* No need to allow visitors to comment on blog posts
* No need for pages like Case Studies, White Papers, Forum, Release Notes, Customers and Partners yet.

# Technical Considerations
Some technical considerations we have to take into account:
* Should we choose WordPress as our CMS framework?
* What is the best CSS framework for responsive web design?
* What is the most cost-effective hosting service?
* How to deploy new code by only 1 click?
* How do we secure the website?