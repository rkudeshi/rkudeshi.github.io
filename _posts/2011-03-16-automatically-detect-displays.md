---
title: Automatically Detect Displays in Mac OS X using AppleScript
date: 2011-03-16
old-slug: automatically-detect-displays
layout: post
---

<p>If you&#8217;re anything like me, you need a large display to be productive (I used a 24-inch LCD when I lived at home and was later spoiled by using <a href="http://twitter.com/probablydan">Dan Tran&#8217;s</a> 30-inch monstrosity when I was in Seattle).</p>
<p>Fortunately, Mac OS X has great support for multiple displays. However, one weird quirk I am often frustrated by occurs when you initially connect the external display to a MacBook or other laptop.</p>
<p>If you do it the proper way, the MacBook should still be sleeping (or turned off) when you connect the Mini DisplayPort (or DVI, for older models) cable to your laptop. However, in Mac OS X 10.5 (Leopard) and 10.6 (Snow Leopard), my MacBook Pro would never automatically register that a new display has been connected and turn it on accordingly.</p>
<p>Hence, I would have to manually go to System Preferences each time I connected the external display (a very frequent occurrence personally, as I took my laptop to school everyday), go into the Displays preference pane, and then manually click on the &#8216;Detect Displays&#8217; button.</p>
<p><a href="/silo/2011/System-Preferences-Displays.png"><img class="size-full wp-image-354 aligncenter" title="System Preferences - Displays" src="/silo/2011/System-Preferences-Displays.png" alt="" width="500" height="428" /></a></p>
<p><a href="/silo/2011/System-Preferences-Detect-Displays.png"><img class="size-full wp-image-355 aligncenter" title="System Preferences - Detect Displays" src="/silo/2011/System-Preferences-Detect-Displays.png" alt="" width="500" height="413" /></a></p>
<div>Eventually, I decided this simple action HAD to be scriptable and looked into AppleScript to figure out a way to do it. Suffice it to say, I tried a bunch of different methods, without satisfying results. Eventually, some adept Googling and a lot of experimentation led me to (in my opinion) the simplest and best code for automating this simple action.</div>
<p>Please note that all credit for the final code goes to <a href="http://www.insanelymac.com/forum/index.php?showtopic=45697">&#8216;Fess&#8217; from the InsanelyMac forums</a>. I&#8217;m just posting this here as a permanent and convenient reference for anyone else who runs into the same problem.</p>
<p>Set up an AppleScript with the following code:</p>
<p><code>tell application "System Preferences" to activate<br />
tell application "System Events"<br />
&nbsp;&nbsp;&nbsp;&nbsp;tell process "System Preferences"<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;click menu item "Displays" of menu "View" of menu bar 1<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tell button "Detect Displays" of window 1 to click<br />
&nbsp;&nbsp;&nbsp;&nbsp;end tell<br />
end tell<br />
tell application "System Preferences" to quit</code></p>
<p>Please note that you have to save this script as a &#8220;.app&#8221; file or otherwise it won&#8217;t work. If you&#8217;re not sure how to do this, <a href="http://www.tuaw.com/2008/01/13/applescript-saving-scripts/">TUAW has a great tutorial</a>.</p>
<p>To activate this script especially quickly, I named my app &#8220;Detect Displays.app&#8221; (original, right?) and use LaunchBar to open it (I set it to the keystroke shortcut &#8220;dd&#8221;).</p>
<p>This simple script has saved me untold time and I hope it does the same for you!</p>

---

If you’re anything like me, you need a large display to be productive (I used a 24-inch LCD when I lived at home and was later spoiled by using [Dan Tran’s](http://twitter.com/probablydan) 30-inch monstrosity when I was in Seattle).

Fortunately, Mac OS X has great support for multiple displays. However, one weird quirk I am often frustrated by occurs when you initially connect the external display to a MacBook or other laptop.

If you do it the proper way, the MacBook should still be sleeping (or turned off) when you connect the Mini DisplayPort (or DVI, for older models) cable to your laptop. However, in Mac OS X 10.5 (Leopard) and 10.6 (Snow Leopard), my MacBook Pro would never automatically register that a new display has been connected and turn it on accordingly.

Hence, I would have to manually go to System Preferences each time I connected the external display (a very frequent occurrence personally, as I took my laptop to school everyday), go into the Displays preference pane, and then manually click on the ‘Detect Displays’ button.

![System Preferences - Displays](/silo/2011/System-Preferences-Displays.png)

![System Preferences - Detect Displays](/silo/2011/System-Preferences-Detect-Displays.png)

Eventually, I decided this simple action HAD to be scriptable and looked into AppleScript to figure out a way to do it. Suffice it to say, I tried a bunch of different methods, without satisfying results. Eventually, some adept Googling and a lot of experimentation led me to (in my opinion) the simplest and best code for automating this simple action.

Please note that all credit for the final code goes to [‘Fess’ from the InsanelyMac forums](http://www.insanelymac.com/forum/index.php?showtopic=45697). I’m just posting this here as a permanent and convenient reference for anyone else who runs into the same problem.

Set up an AppleScript with the following code:

`tell application "System Preferences" to activate
tell application "System Events"
    tell process "System Preferences"
        click menu item "Displays" of menu "View" of menu bar 1
        tell button "Detect Displays" of window 1 to click
    end tell
end tell
tell application "System Preferences" to quit`

Please note that you have to save this script as a “.app” file or otherwise it won’t work. If you’re not sure how to do this, [TUAW has a great tutorial](http://www.tuaw.com/2008/01/13/applescript-saving-scripts/).

To activate this script especially quickly, I named my app “Detect Displays.app” (original, right?) and use LaunchBar to open it (I set it to the keystroke shortcut “dd”).

This simple script has saved me untold time and I hope it does the same for you!