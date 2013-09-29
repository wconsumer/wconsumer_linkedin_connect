Connect with Linkedin (wconsumer)
========================

Implements "Connect with Linkedin" feature allowing user to sign in or sign up with his Linkedin account. 

User flow is as follows:

1.  User clicks Connect with Linkedin link in login form.
1.  Module authenticates user with Linkedin and retrieves his Linkedin account data.
1.  If there is a user registered in Drupal having same Linkedin url ('html_url' field of Linkedin /user response) then user is logged in with this account.
1.  If there is no such account then try to register user with his Linkedin login and email.
1.  If registration fails (login or email already taken, etc) then redirect user to the register page and allow him to manually register a new account.
