
## Basic Email Template

Copy the index file into an email delivery service of your choice (SendGrid, Mailchimp), replacing placeholder images and body text with content. Update the href of the button as it currently points to WePresent. If the email body color needs to change, find all instances of #EDEBE9 and replace.

The email is broken up into the following sections:

* Hidden preview text
* Header logo
* Hero image
* Body text
* Button
* Footer
    * Signature
    * Footer logo
    * Footer text
    
The "view in browser" link and "here" unsubscrible link are currently set up for SendGrid. If using another email delivery service, replace the [weblink] and [Unsubscribe] in the href quotes with whatever another email delivery service requires.

The reason this template was made was to solve some limitations of the provided templates from SendGrid. Currently the only unresolved issue is the border-radius property not being accepted by Outlook 2000, 2002 and 2003 on Windows 7. On these clients the button will appear with hard edges.

The template has the following properties:

Ariel and Helvetica as fonts.
Edge to edge body color in all mail clients that support this.
Fixes for centring issues on Gmail app in iOS 10 and 11.
Fixes for border-radius on buttons in Outlook with the exception of the versions listed above.
This template has been run through Litmus and passes all tests, though when the placeholder content is replaced, please run through Litmus to assure no bugs have occured. Outlook 2016 on Windows 7 will occasionally place a 1px white line under some content. If this line appears, try to make sure any image, gif or body text added to the template is not more than 700px in height. If that does not solve the problem, try adding the following code directly under the affected content's closing tag:
```
<!--[if gte mso 12]>
  <br/>&nbsp;
<![endif]-->
```
If this doesn't work, please Google another solution, there are quite a few options to try :)
