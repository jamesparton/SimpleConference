Simple Conference
=================

This repro demonstrates just how easy it is to get up and running with Twilio voice.
To create a simple, but feature rich, conference call room you just need 7 lines of Twiml (Twilio's XML schema)

You can read the Twilio "HowTo" doc on conferencing here: http://www.twilio.com/docs/howto/simple-conference

Preparation
===========

Open an account on http://twilio.com<br>
Buy a phone number in your country of choice http://www.twilio.com/docs/howto/search-and-buy

Creating the conference room
============================

Use the XML document contained in this repo.<br>
You only need to make one edit to the XML. Just switch the <code>Conference waitUrl</code> value to point to the MP3 track you want to play as your wait music.<br>
Upload the XML doc to your server, or a hosting service like Twimlbin - http://twimlbin.com/4a1fb535<br>

<p>This conference room will play hold music until at least two people are in the room, and will also make a recording of the call.

Configuring your Twilio number
==============================

Once you have uploaded your XML document you just need to tell Twilio what to do when someone calls your number.<br>
Sign into your account on http://twilio.com and click on 'Numbers' in the navigation at the top of the page.<br>
Find the number you want your conference room to hang from and click on it.<br>
In the 'Voice Request URL' field type in the URL where you stored your XML.<br>
Click the 'Save Changes' button<br>

<p>That's it you're done!

Pointing Multiple Numbers To The Same Conference
================================================

You may wish to provide local dial numbers in multiple countries to save your callers having to make expensive international calls.<br>
This is simple to achieve.<br>
Just buy additional Twilio numbers in the countries you need and repeat the 'Configuring your Twilio number' step for all the new numbers. When your callers dial their local number, they will all be directed into the same common confernece room.

Retrieving Call Recordings
=========================

You can retrive call recordings from your Twilio account.<br>
Sign into your account on http://twilio.com and click on 'Logs' in the navigation at the top of the page<br>
Then click on 'Recordings'<br>


Useful Links
============

All things Twilio - http://twilio.com<br>
Twilio technical docs - http://twilio.com/docs<br>
Need help? - http://forum.twilio.com/twilio/<br>
Need inspiration? - http://twilio.com/gallery/customers<br>
Need a Twilio coder? - http://twilio.com/doers<br>
Want to work for Twilio in Europe? - http://bitly.com/bundles/jamesparton/3
