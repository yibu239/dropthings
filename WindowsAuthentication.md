# Introduction #

You can change the login page to use Windows Authentication instead of ASP.NET Authentication.


# Details #

Dropthings needs the ASP.NET Membership tables and API to function. So, you can't replace the authentication mode from forms to windows. It needs the ASP.NET Membership stuffs to support the anonymous mode.

Now, if you want to keep the anonymous browsing feature intact and just want to offer login using windows authentication then you need to just change the Membership.ValidateUser call in Login.aspx with Windows Authentication code to validate the username and password. Once that is done, the rest of the code where the Membership.CreateUser call is, then issuing FormsAuthentication ticket etc needs to remain.

If you want to totally disable anonymous browsing feature and allow only authenticated windows users to visit the site then first of all you need to keep the current forms authentication as is, but implement a check for logged in user in Default.aspx page load. If there's no user logged into browser, then you need to redirect user to login.aspx. You can find the detail guide here:
http://msdn.microsoft.com/en-us/library/ms972958.aspx

There's some IIS tweaking you need to do.

I haven't personally tried this. So, you will have to try it out based on how your environment is configured.