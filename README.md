hide referer
=============
This scipt hides the referer when clicking a link by redirecting to this script and re-redirecting to the prefered site. This is a minimal script written just in some lines of js. Normally the redirect destination is written as an anchor at the end of the URL. Because of this, the destination is never transmitted to the server (unless the code is compromised and it is sent to the server by js). Sadly the anchor seems to get removed on a 302/301-redirect on Safari. Because of this, a ?...-Fallback was added in V1.4. There, the destination is transmitted to the server.

The URLs will look like this: [https://thomas131.github.com/hide_referer/#https://example.com](https://thomas131.github.com/hide_referer/#https://example.com)

The GET-Fallback will look like this: [https://thomas131.github.com/hide_referer/?https://example.com](https://thomas131.github.com/hide_referer/?https://example.com)
Forks, reuploads, ... are more than welcome to make this tool more decentrialized.

This code is licensed as [![image](https://licensebuttons.net/p/zero/1.0/88x31.png "CC0")](https://creativecommons.org/publicdomain/zero/1.0/).

Why not a 302-Redirect?
-----------------------
For sure, 302-redirects have lots of advantages (less overhead, no JS, ...) but they have at least one disatvantage: The Server knows the source (refferer) and the destination. The less data the server has, the less data can be stolen. Additionally I can't do 302-redirects in a GitHub Page.
