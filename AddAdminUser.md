# Introduction #

From Dropthings 2.5, we have introduced "admin" role which can access pages inside the /admin folder. Here's how you create the admin role and user.


# Details #

On Visual Studio Solution Explorer, while you have the Dropthings web project selected, you will see a button that says "ASP.NET Configuration". Click that. It will launch a website where you can add new role. Add a new role named "admin", exactly the "admin".

Then add a new user "admin" and put that user in the admin role.

You can then login to Dropthings and hit any page like /admin/managewidgets.aspx and login as the admin user.