# Problem #
Dropthings needs some default rows to be in certain tables. Otherwise it cannot run. So, if you have taken the Dropthings database from the project and then you have removed all rows from the tables, then the site will not work. You will get blank tabs.

# Solution #

After copying a Dropthings database that runs perfectly fine, you need to run the "Resurrection" stored proc. It will cleanup all users (anon or registered) except the template users define in the stored procedures. The empty database will then be ready for production use.