# dial - a - dpla

!SLIDE marker

# Dial - A - DPLA
## Mx A. Matienzo
###Digital Public Library of America

!SLIDE marker

# Hi!

!SLIDE marker

## I spent a short amount of time with [Twilio](http://twilio.com/)

!SLIDE marker

## Twilio allows you to make and receive phone calls, and send and receive SMS messages
### ... using REST (yay!)

!SLIDE marker

## Twilio's not new to Code4lib
### (see [Mike Beccaria's 2011 C4LJ article](http://journal.code4lib.org/articles/5542))

!SLIDE marker

# And it can be F—U—N

!SLIDE marker

## Dial - A - DPLA provides access to sound items in DPLA.

!SLIDE marker

# Live demo (eek!)

!SLIDE marker 

# Call +1 704 288-DPLA
## (+1 704 288-3752)

!SLIDE marker

## [50 line Python (Flask) app](https://github.com/anarchivist/dial-a-dpla/blob/master/dial_a_dpla/app.py) using Twilio API using sample records from Kentucky Digital Library through DPLA API.

!SLIDE marker

## Serves simple TwiML (XML) data and handles POST requests

!SLIDE marker

<pre>&lt;?xml version="1.0" encoding="UTF-8"?&gt;
&lt;Response&gt;
	&lt;Say&gt;Welcome to Dial a D P L A!&lt;/Say&gt;
	&lt;Gather action="lookup" method="POST" numDigits="4"&gt;
		&lt;Say&gt;Please enter a four digit year followed by the pound key.&lt;/Say&gt;
	&lt;/Gather&gt;
&lt;/Response&gt;
</pre>

<pre>
&lt;?xml version="1.0" encoding="UTF-8"?&gt;
&lt;Response&gt;
	&lt;Say&gt;You are about to listen to: Sullivan in Germany.&lt;/Say&gt;
	&lt;Say&gt;This item is from University of Kentucky.&lt;/Say&gt;
	&lt;Play&gt;http://[redacted].mp3&lt;/Play&gt;
&lt;/Response&gt;
</pre>

!SLIDE marker

# Thanks!
## @anarchivist
#### https://github.com/anarchivist/dial-a-dpla
