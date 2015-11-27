Do you trust that certificate?
------------------------------
A [rabbit](http://rabbit-shocker.org/) presentation.

= Usage
Install rabbit and run `rake` 

= Abstract
Some developers don't seem to take too much care of which CA certificates they trust when connecting to external services from their web apps. Certificates may come with the OS the app is running on or Ruby gems the app depends upon. This is not secure nor good for continued operation of the app. I will try to let the listeners know this fact and request to think the best way to maintain certificates depending upon the needs of their apps.

= Details
The outline of the presentation is currently:

- An example of gems that comes with CA/intermediate SSL certificates
- The fact that I saw some apps with old gems on Heroku stopped working when external services retired certificates signed with SHA-1
- This might happen again [if Google invalidates certificates by Symantec on June 1st, 2016](https://googleonlinesecurity.blogspot.com/2015/10/sustaining-digital-certificate-security.html)
- OSs also have installed certificates
- How vanilla `openssl/ssl.rb` locates those certificates
- How some gems change locations of certificates
- How this maybe monkey patched

I hope to communicate to developers of web apps, especially of those handles payment information, that they should be aware of what they trust when developing an app. This should make the app more secure and make the developers aware of when to update gems or certs.
