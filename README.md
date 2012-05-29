# jquery.cookieBar

A simple, lightweight jQuery plugin for creating a notification bar that is dismissable and dismiss is saved by cookie. Perfect for implementing the new eu cookielaw!

Uses: [jQuery.Cookie](https://github.com/carhartl/jquery-cookie) - bundled, no need to reference.

## Installation

Include script *after* the jQuery library

    <script src="/path/jquery.cookieBar.js"></script>

## Usage

Create your cookiebar markup from a simple container, example:

	<script type="text/javascript">
		$(document).ready(function() {
		  $('.cookie-message').cookieBar();
		});
	</script>
	
	<div class="cookie-message">
		The government says i have to tell you i use cookies, so here it is
    </div>
	
Create your cookiebar markup from a simple container with an advanced button, example:

	<script type="text/javascript">
		$(document).ready(function() {
		  $('.cookie-message').cookieBar({ closeButton : '.my-close-button' });
		});
	</script>
	
    <div class="cookie-message">
		The government says i have to tell you i use cookies, so here it is <a class="my-close-button" href>cheers!</a>
	</div>

Full Example
	Check out [example.html] (example.html)
	
## Options

    closeButton: 'none'

Define a close button for the bar, if undefined or 'none' a close button will be added automagically

	secure: true
   
If set to true transmission requires secure protocal (https), default: false.
 
	path: '/path/for/cookie'

Path the cookie is valid for, default: '/' (site wide)
  
## Authors

[Carl Woodhouse](https://github.com/carlwoodhouse)
