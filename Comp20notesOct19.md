JQUERY - Solved problem for crappy browser support

<!DOCTYPE html>
<html>
<head>
	<title>Simple Jquery</title>
	<script src="jquery script source">
		$(document).ready(function(){
			//Regular JS way of modifying text
			document.getElementById("schedule").innerHTML = "Signal Problems";

			//JQuery method of modifying text
			$("schedule").html("Signal Problems");
		});
	</script>
</head>
<body>
	<h1>Red Line Train Schedule</h1>
	<div id="schedule">Find the schedule here</div>
</body>
</html>



Jquery:
.ready(): specify function to execute when DOM is fully loaded

Storing data over time(persistently)
How does your browser remember who you are
This is done using cookies and cache

Storing Data Persistently:
Cookies: One cookie == 4 kilobytes of data
~300 cookies max per site
A cookie is a key value pair
1 major downside: It can be modified(HowTo?)
Cookies are used to leave a trail
Go to application to view cookies for site

RFC Cookies - Request for comments
RFC 6265 - Standard for cookies

All cookies per site must be sent with every http request
Cookies are stored on your file system
Now use get request to retrieve cookies

Lcoal Storage(cache)
No key value pair limit
~5mb of storage per site
Still key value pair
Can be modified
Local storage data is not sent with every http request

Online bank cannot read cookies from local machine to server
Most sites store cookies
One site cannot read cookies of another site