# slack-theme
A dark theme for slack

At the time of this writing, Slack was using jQuery. So, easiest thing to do is fire some $.ajax() to get a publicly available theme as a starting point, then combine that with some of your own tweaked styles, then inject into Slack's DOM.

Open
(OSX): /Applications/Slack.app/Contents/Resources/app.asar.unpacked/src/static/ssb-interop.js
(Linux {thanks @svenwoldt}): /usr/lib/slack/resources/app.asar.unpacked/src/static/ssb-interop.js
(Windows): %LocalAppData%\Slack<latest>\resources\app.asar.unpacked\src\static\ssb-interop.js
(Linux Mint 19 {thanks @stevenc7}): /var/lib/flatpak/app/com.slack.Slack/current/active/files/extra/lib/slack/resources/app.asar.unpacked/src/static/ssb-interop.js

Then drop this code at the bottom of the above file (note that as of 11.7.18 there is a conditional statement you'll want to put this code inside of, so just put the below right before the enclosing curly brace).
