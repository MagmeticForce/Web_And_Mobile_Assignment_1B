# Web_And_Mobile_Assignment_1B

## Section 1: The Less-than-equal-4-Click User Journey Funnel
* Starting state: user lands on the page and identifies the primary signifier (links, logo, high-contrast “Deploy Free Cluster” CTA)
* Step 1: user scrolls to the pricing tiers or clicks “Deploy Free Cluster.” Upon scrolling, they will encounter the key platform capabilities such as Latency Tracking, Auto-Remediation, and Log Aggregation.
* Step 2: user compares the “Developer,” “Pro Cluster” and “Enterprise Detailed” tiers, where the most popular of the three visually stands out via a visual badge.
* Step 3: user fills out pre-registration form in order to receive API sandbox provisioning details, including numeric bounds for verifying tier compatibility.
* Step 4: user presses the “Submit Form” button.
* Terminal State: confirmation pop-up displays telling the user that their response has been received.

## Section 2: Don Norman Usability & Constraint Audit
* Normal principle 1:
  * Signifier 
  * Primary Action Button (Above the fold)
  * Then anchor tag <a> is used to signify that an element is clickable navigation. CSS Stylings can further be used to make the element look like a button.
* Normal principle 2:
  * Signifier 
  * Recommended Tier Indicator 
  * The <div> tag is used to add a tag on the Pro Cluster tier card, highlighting that it is the most popular option. The other two pricing cards lack this tag, making the Pro Cluster card stand out.
* Norman principle 3:
  * Physical/System Constraint 
  * Workload Estimator: Node Count
  * The <input> tag with attributes min and max enforces the numerical limits. Additionally, the step attribute can be defined so that the user can use up/down arrows to increase/decrease the value and ensure they stay within numeric bounds.
* Normal principle 4:
  * Physical/System Constraint 
  * Operator Contact Field 
  * The <input> tag’s required field ensures that there are no blank responses. Since this is a boolean attribute, simply including it in the tag indicates a value of true.
* Normal principle 5:
  * Feedback Loop
  * Form Submission / Live
  * Anchors
  * Confirmation text displays, notifying the user that their response has been recorded. If possible, the button for submission grays out and is no longer functional.


## Section 3: Semantic Component & Layout Tree
Body
  Header
    a (brand logo)
    nav
      a (features link)
      a (pricing matrix)
      a (form)
      a (“Deploy Free Cluster” CTA)
  Main
    section (hero)
      Header
        h1
        p (subtitle)
      Div
        p (body text)
        a (“Deploy Free Cluster” CTA)
    section (features)
      Header
        h2
        p
      div
        article (Latency Tracking)
          h3 
          ul
            li
            li
            li
        article (Log Aggregation)
          h3
          ul
            li
            li
            li
      article (Enterprise Dedicated)
        h3
        ul
          li
          li
          li
    section (pricing tiers)
      Header
        h2
        p
      div
        article (Developer tier card)
          h3
          p
          ul
            li
            li
            li
          a
        article (Pro Cluster card)
          div (“Most popular” tag)
          h3
          p
          ul
            li
            li
            li
          a
        article (Enterprise Dedicated card)
          h3
          p
          ul
            li
            li
            li
          a
    section (form)
      Div (form wrapper)
        header
          h3
          p
        form
          div
            label
              span (required mark)
            input (type=”email”, required)
          div
            label
              span (required mark)
            input (type=”number”, min, max, step, required)
            span (hint for numeric limits)
          div
            label
              span (required mark)
            select (required)
              option
            option
            option
          div        
            button
  Footer
    a (brand logo)
    p (copyright)
    nav
      a (back to top)
      a (features)
      a (pricing matrix)
      a (“Deploy Free Cluster” CTA)

