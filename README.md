Do you trust that certificate?
------------------------------
A [rabbit](http://rabbit-shocker.org/) presentation presented as a [Lighting Talk at RubyKaigi 2015](http://rubykaigi.org/2015/presentations/lt).

I hope to communicate to developers of web apps, especially of those handles payment information, that they should be aware of what they trust when developing an app. This should make the app more secure and make the developers aware of when to update gems or certs.

## Usage
Install rabbit and run `rake` 

## Abstract
Some developers don't seem to take too much care of which CA certificates they trust when connecting to external services from their web apps. Certificates may come with the OS the app is running on or Ruby gems the app depends upon. This is not secure nor good for continued operation of the app. I will try to let the listeners know this fact and request to think the best way to maintain certificates depending upon the needs of their apps.

## License
CC BY-ND 4.0

Copyright 2015 by zunda <zundan at gmail.com>
