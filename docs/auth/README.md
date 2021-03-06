# User Authentication

Handling user authentication is difficult. Deploying it serverlessly is an
added challenge. This should help you transition away from using `express-session`
as well as `passport.session()`, as these don't work nicely in a stateless
environment. Instead, we'll be passing JWTs with our requests!

This guide assumes you've already gone through [this tutorial with Google OAuth](https://medium.com/@maartendebaecke2/mern-stack-implementing-sign-in-with-google-made-easy-9bfdfe00d21c).
If this isn't the case, all you need to know from that is how to set up an
OAuth Consent Screen, as well as getting a Client ID and a Client Secret from
the [APIs & Services page](https://console.cloud.google.com/apis) of Google's
Cloud Platform. After that's all good, we can make the changes we need!

There's a good amount of stuff going on, so it's broken up over the following
pages. If you follow it top to bottom, you should be good!

**Backend**
 - [Migrating from sessions to JWTs](auth/backend?id=migrating-from-sessions-to-jwts)
 - [Endpoints and middleware to authenticate](auth/backend?id=endpoints-and-middleware)
 - [Configuring networking stuff](auth/backend?id=configuring-networking-stuff)

**Frontend**
 - [Passing credentials to the API](auth/frontend?id=passing-credentials-to-the-api)
 - [Logging in/out](auth/frontend?id=logging-inout)
 - [Getting the user](auth/frontend?id=getting-the-user)

**Google OAuth**
 - [Moving to production](auth/google-oauth)
