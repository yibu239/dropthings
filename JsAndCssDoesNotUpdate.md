# Introduction #

Dropthings caches JS and CSS on browser as well as on ASP.NET Cache.

# Details #

If you want to see changes made in JS or CSS, then you need to go to web.config and increase the CssVersionNo and JsVersionNo so that server cache is flushed and browser gets the new stuff.

If you have 2.5.4 or above, there's a DeveloperMode setting, which stops all caching.