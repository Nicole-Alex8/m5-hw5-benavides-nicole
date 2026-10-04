# m5-hw5-benavides-nicole

Accessibility Audit

I used Lighthouse, WAVE, and VoiceOver to audit the website for accessibility issues.


Initial Audit — Issues Found
The accessibility tools identified the following issues:
    Lighthouse
        - Accessibility score: 91% 
        - Insufficient color contrast
        - Headings aren't in sequential order
        - No main landmark
    WAVE
        - 3 missing form labels
        - 12 very low contrast errors
        - 1 missing page region
        - 1 skipped heading level
    VoiceOver
        - h3 was annouced twice
    Keyboard Accessibility
        - when tabbing through I noticed that the Message box wouldn't highlight in blue


Accessibility Fixes

I made the following changes base on the audit results:
    - Color contrast: Fixed body, navigation and footer text: #0c0c0c; | Fixed "Internet Andrea" text: rgb(219, 51, 234);| Fixed navigation and footer background color: #d86fef;
    - Heading structure: replaced <h3> with <h2> for the About Me and Reach out for a quote today! headers
    - Form labels: Adding proper HTML <label> for Name, Email, and Message. | Adding id="" in between input and placeholder. 
    - Creating a button: replacing <div class> with <button type>
    - Main page region: Wrapped the primary page content (hero, about section & contact form) using <main>
    - Keyboard Accessibility: I removed the textarea:focus { outline: none; } CSS style function


Final Audit

After making the changes, I ran the website through Lighthouse and WAVE again and tested the website using VoiceOver. Accessibility score via Lighthouse: 100%. Zero errors on WAVE. VoiceOver was staightforward. The accessibility issues identified during the inital aduit were resolved.