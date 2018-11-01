---
title: This is a test file

---

<p>Steps to config ARR as a Proxy Server for AutoACME</p>
<p>1/ Go to ARR Cache, then Server Proxy Setti<img src="https://lh3.googleusercontent.com/3Y20WQEoez786KY1D4f0uWLfXN42-YVnWkr-0CV8IHGYKrzhZFcJW0JElGHzAUFPFWPgDvT80-78" alt="Good photo">ngs</p>
<p>2/ Check on Enable proxy</p>
<p>3/ Create a site call AutoACME and add a binding to support <a href="http://autoacme.com">autoacme.com</a> port 80</p>
<p>4/ Go to URL Rewrite</p>
<p>5/ Add a blank rule under Inbound and put Pattern = .well-known/acme-challenge/(.*)</p>
<p>Rewrite URL = <a href="http://autoacme.com/%7BR:1%7D">http://autoacme.com/{R:1}</a></p>
<p>6/ In hosts file, add <a href="http://autoacme.com">autoacme.com</a> to point to IP of current server</p>
<p>7/ Add a file into folder of AutoACME site and it</p>
<p>8/ Go to Centralized Certificates / Edit Feature Settings</p>
<p>9/ Config it, points to a localtion which will be used by AutoACME + the CPKP password which AutoACME will encrypt</p>

