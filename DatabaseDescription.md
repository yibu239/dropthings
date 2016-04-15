Dropthings has the following tables:


  * aspnet\_Users - ASP.NET Membership table that holds the user accounts, both anonymous and registered.
  * aspnet\_membership - ASP.NET Membership table that holds the registered user account details.
  * aspnet\_Profile - ASP.NET Profile that holds Profile information for each user. For ex, whether it's the first visit of the user or not.
  * aspnet\_Roles - ASP.NET Roles. Two mandetory roles that must be in the database are "Guest" and "Registered".
  * Widget - The definition of widgets.
  * WidgetsInRoles - Mapping between Widget and aspnet\_Roles that decides which roles can see which widgets. For example, only RegisteredUsers role can see certain widgets which guest users cannot see.
  * Page - The tabs of a user. User can have one or more tabs.
  * Column - Columns on a page. A page can have 1 to 3 columns.
  * WidgetZone - Container for widget instances. Each column has one widgetzone.
  * WidgetInstance - Represents an instance of a widget in a certain widgetzone.
  * Token - Used to store some temporary information that's valid for a certain time. For example, account activation key.
  * RoleTemplate - It maps the roles that belongs to the template users. These roles are automatically given to newly created users when their tabs and widgets are created from the template user defined in web.config.