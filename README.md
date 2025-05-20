# CSE110-Lab7

#### Team member: Fong Yu Lin

### "Check Your Understanding" questions

1. Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

   a. Within a Github action that runs whenever code is pushed\
   b. Manually run them locally before pushing code\
   c. Run them all after all development is completed\

   **Answer:**\
    I would fit my automated tests within a Github action that runs whenever code is pushed. Since it's `automated tests`, it should not be run manually. They are meant to verify code correctness automatically and consistently.

2. Would you use an end to end test to check if a function is returning the correct output? (yes/no)

   **Answer:**\
   No, end to end test is supposed to test the user interaction with the webpage rather than the accuracy of the output. Unit tests are more appropriate for verifying the output of specific functions because they are faster, more focused, and easier to debug.

3. What is the difference between navigation and snapshot mode?

   Navigation mode provides an overall performance metric but cannot analyze the interactions or change in content. It is useful for analyzing load performance but does not reflect dynamic state changes after initial load.

   Whereas snapshot mode analyzes the current static state of a rendered page. It captures a "snapshot" without going through the full navigation process, making it ideal for checking accessibility. However, it does not measure load performance or JS execution time.

4. Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

   **Accessibility (Score: 90)**\
   Add a `lang` attribute to the `<html>` tag to help screen readers and assistive technologies interpret the content correctly.

   **Best Practices (Score: 96)**\
   Include a `<meta name="viewport">` tag in the HTML to ensure the site is responsive on mobile devices and to eliminate the default 300ms input delay.

   **SEO (Score: 91)**\
   Add a meta description tag (`<meta name="description" content="...">`) to provide search engines with a concise summary of the page, which can improve visibility in search results.
