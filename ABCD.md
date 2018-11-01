---
title: Steps to config ARR as a Proxy Server for AutoACMEThis is a test file

---

<h1 id="steps-to-config-arr-as-a-proxy-server-for-autoacme">Steps to config ARR as a Proxy Server for AutoACME</h1>
<p>1/ Go to ARR Cache, then Server Proxy Settings</p>
<p>2/ Check on Enable proxy</p>
<p>3/ Create a site call AutoACME and add a binding to support <a href="http://autoacme.com">autoacme.com</a> port 80</p>
<p>4/ Go to URL Rewrite</p>
<p>5/ Add a blank rule under Inbound and put Pattern = .well-known/acme-challenge/(.*)</p>
<p>Rewrite URL = <a href="http://autoacme.com/%7BR:1%7D">http://autoacme.com/{R:1}</a></p>
<p>6/ In hosts file, add <a href="http://autoacme.com">autoacme.com</a> to point to IP of current server</p>
<p>7/ Add a file into folder of AutoACME site and it</p>
<p>8/ Go to Centralized Certificates / Edit Feature Settings</p>
<p>9/ Config it, points to a localtion which will be used by AutoACME + the CPKP password which AutoACME will encrypt</p>

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2ODU4NTkyN119
-->