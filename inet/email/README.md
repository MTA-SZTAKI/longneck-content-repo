inet/email
==========
Transformation rules for [emails](http://en.wikipedia.org/wiki/Email), mainly for general and localized email addresses.


###email.entity.xml
Contains the definition of an email address, according to the [W3C standard](http://www.w3.org/Protocols/rfc822/).


###email.block.xml
Cleans and validates email fields according to the entity definition. Single input and output fields are assumed.
No language- or country-specific rules are applied.


###email.double.block.xml
This block can process email fields containing one or two valid email addresses. 
It tries to separate the addresses and then to apply blocks in `email.block.xml`.
