# Read-13

## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS.

#### DIVING IN
ersistent local storage is one of the areas where native client applications have held an advantage over web applications.
***Cookies Disadvantuges:***
* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet
* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

***What we really want is***
* a lot of storage space on the client that persists beyond a page refresh and isn’t transmitted to the server.
* Before HTML5, all attempts to achieve this were ultimately unsatisfactory in different ways.

#### A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5
* In the beginning, there was only Internet Explorer.Microsoft invented DHTML Behaviors, and one of these behaviors was called userData.
* userData allows web pages to store up to 64 KB of data per domain(Trusted domains, such as intranet sites, can store 10 times that amount)
* In 2002, Adobe introduced a feature in Flash 6 the feature is properly known as Local Shared Objects.Briefly, it allows Flash objects to store up to 100 KB of data per domain.
* In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers. After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.
* By 2009, dojox.storage could auto-detect Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.
* Despite heroic efforts to paper over the differences (in dojox.storage), they all expose radically different interfaces, have different storage limitations, and present different user experiences. So this is the problem that HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

#### INTRODUCING HTML5 STORAGE
* What I will refer to as “HTML5 Storage” is a specification named Web Storage, So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser.
* Unlike cookies, this data is never transmitted to the remote web server
* Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

#### USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript.

***TRACKING CHANGES TO THE HTML5 STORAGE AREA***
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.

***LIMITATIONS IN CURRENT BROWSERS***
 limitations of the now-standardized HTML5 Storage. The answers, in order of importance, are `5 megabytes,` `QUOTA_EXCEEDED_ERR,` and `no.`
`5 megabytes,` is how much storage space each origin gets by default.
`QUOTA_EXCEEDED_ERR,` is the exception that will get thrown if you exceed your storage quota of 5 megabytes.
`no.` is the answer to the next obvious question, `Can I ask the user for more storage space?`.

#### HTML5 STORAGE IN ACTION
with HTML5 Storage, we can save the progress locally, within the browser itself. Here is a live demonstration.

#### BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices.
