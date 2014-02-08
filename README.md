# single-page-login

A meteorite package for a Bootstrap 3 Googlesque login, sign up and password reminder form and functionality.

# Meteor Dependencies

* accounts-password
* accounts-ui

# Meteorite Atmosphere Dependencies
* [iron-router](https://atmosphere.meteor.com/package/iron-router "iron-router")
* [bootstrap-3](https://atmosphere.meteor.com/package/bootstrap-3 "bootstrap-e")

# Installation

    mrt add single-page-form

# Configuration

* loginTitle: Sets the title on the login page.
* signupTitle: Sets the title on the sign up page.
* forgotPasswordTitle: Sets the title on the retrieve password page.
* canRetrievePassword: Boolean. Turns on/off password retrieval page and functionality.
* passwordSignupFields: Sets the Meteor Accounts.ui.config passwordSignupFields to USERNAME_AND_EMAIL, USERNAME_AND_OPTIONAL_EMAIL, USERNAME_ONLY, EMAIL_ONLY.
* forbidClientAccountCreation: Boolean. Sets the Accounts.config forbidClientAccountCreation fieild.
* routeAfterLogin: Iron Router route after login.
* routeAfterSignUp: Iron Router route after sign up.
* forceLogin: Boolean.  Forces single page login except for signup and forgot-password routes.

```
  SinglePageLogin.config({
      loginTitle: 'Single page login',
      signupTitle: 'Single page sign up',
      forgotPasswordTitle: 'Retrieve password',
      canRetrievePassword: true,
      passwordSignupFields: 'EMAIL_ONLY',
      forbidClientAccountCreation: false,
      routeAfterLogin: '/dashboard',
      routeAfterSignUp: '/dashboard',
      forceLogin: true,
  });
```

# Out of the Box Iron Router Routes
* /signup
* /login
* /forgot-password

# License
Copyright (c) 2013 [EtherPOS](http://www.etherpos.com/ "EtherPOS, LLC"). Released under an MIT license.
