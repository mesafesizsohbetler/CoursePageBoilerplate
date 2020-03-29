 
<div id="text"></div>
 
<script>
document.getElementById("text").innerHTML = "Text added by JavaScript code";
 var ifrm = document.createElement('iframe');
		ifrm.setAttribute('id', 'ifrm'); // assign an id

		// to place before another page element
		var el = document.getElementById('site-footer-owner');
		el.parentNode.insertBefore(ifrm, el);

		// assign url
		ifrm.setAttribute('src', 'http://google.com');
</script>
