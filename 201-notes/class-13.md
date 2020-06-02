## “The Past, Present, and Future of Local Storage for Web Applications”

**Diving In**

- downside of cookies for local storage

  1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

  2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)

  3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

- What we really want is

  1. a lot of storage space on the client
  2. that persists beyond a page refresh 
  3. and isn’t transmitted to the server

**HTML5 Storage**

- it’s a way for web pages to store named key/value pairs locally, within the client web browser


[Back to Homepage](https://ashcaz.github.io/reading-notes)