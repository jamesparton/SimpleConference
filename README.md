Simple Conference
=================

This repro demonstrates just how easy it is to get up and running with Twilio voice.
To create a simple, but feature rich, conference call room you just need 7 lines of Twiml (Twilio's XML schema)

You can read the Twilio "HowTo" doc on conferencing here: http://www.twilio.com/docs/howto/simple-conference

Preparation
===========
<ul>
<li>Open an account on http://twilio.com</li>
<li>Buy a phone number in your country of choice http://www.twilio.com/docs/howto/search-and-buy</li>
</ul>

Creating the conference room
============================
<ul>
<li>Use the XML document contained in this repo. You only need to make two edits to the XML.</li>
<li>Edit 1: In the <code>Say</code> line replace [Your Name] with the name to be played to callers.</li>
<li>Edit 2: Switch the <code>Conference waitUrl</code> value to point to the MP3 track you want to play as your wait music.</li>
<li>Upload the XML doc to your server, or a hosting service like Twimlbin - http://twimlbin.com/</li>
</ul>

This conference room will play hold music until at least two people are in the room, and will also make a recording of the call.

Configuring your Twilio number
==============================
<ul>
<li>Once you have uploaded your XML document you just need to tell Twilio what to do when someone calls your number.</li>
<li>Sign into your account on http://twilio.com and click on 'Numbers' in the navigation at the top of the page.</li>
<li>Find the number you want your conference room to hang from and click on it.</li>
<li>In the 'Voice Request URL' field type in the URL where you stored your XML.</li>
<li>Click the 'Save Changes' button</li>
</ul>

That's it you're done!

Pointing Multiple Numbers To The Same Conference
================================================
You may wish to provide local dial numbers in multiple countries to save your callers having to make expensive international calls.<br>
This is simple to achieve.<br>
<p>Just buy additional Twilio numbers in the countries you need and repeat the 'Configuring your Twilio number' step for all the new numbers. When your callers dial their local number, they will all be directed into the same common conference room.<br>

Retrieving Call Recordings
=========================
<ul>
<li>You can retrive call recordings from your Twilio account.</li>
<li>Sign into your account on http://twilio.com and click on 'Logs' in the navigation at the top of the page.</li>
<li>Then click on 'Recordings'</li>
</ul>

Useful Links
============

All things Twilio - http://twilio.com<br>
Twilio technical docs - http://twilio.com/docs<br>
Need help? - http://forum.twilio.com/twilio/<br>
Need inspiration? - http://twilio.com/gallery/customers<br>
Need a Twilio coder? - http://twilio.com/doers<br>
Want to work for Twilio in Europe? - http://bitly.com/bundles/jamesparton/3
