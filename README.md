# X-Prefer-Dark-Theme
An initiative for universal support of dark themes on the web.

During the last few years we've seen major support for dark themes everywhere:

* Windows 10 introduced support in the Anniversary Update,
* OS X has support for it since El Capitan (albeit in a hacky way),
* Youtube recently added it,
* and just a few weeks ago Twitter just got it as well.

Currently if you prefer dark themes you have a few options:

* opt-in if the site already supports it (most of these only work after logging in)
* install browser extensions (these often break as the sites are updated)
* write your own user-css in browsers that support it (too much effort, also breaks often)

## Solution - Proposal

Add a new HTTP header "X-Prefer-Dark-Theme" that would be sent out by browsers. In turn, websites / webapps receiving this header would respond with the dark themed variants of their site. In my opinion this would solve many problems:

* universal way to signal for dark theme requested
* a single browser plugin could help until browsers officially add the feature
* later, browsers could even read the OS setting (eg. if the Windows 10 dark theme is enabled automatically enable it in the browser as well)
* leaves the task of solving the issue with the website owners
* provides a measurable way to track how many people want dark theme, boosting its support
* does not require users to log in
* does not require users to find how to enable it on a new site

## Game plan

* Write and submit RFC to make it official
* Convince sites that already offer a dark theme to use the header to automatically opt-in users
* Gather support from other sites & browsers
