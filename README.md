# URN's
##Uniform Resource Names for the Farm Data Standards

The purpose of the urn:nzl:pri: namespace is to support a list of unique identifier namespaces for use within the primary sector. A variety of official biosecurity and genetic recording schemes define identifiers for farms, herds, organisations and animals. A master list of these schemes allows software and device vendors to understand and interpret identifiers in a useful manner.
The NZ Farm Data Standards project is the interim administrator of the urn:nzl:pri: namespace, delegated by the Department of Internal Affairs of the New Zealand Government, consistent with [RFC-4350](https://www.ietf.org/rfc/rfc4350.txt). It is charged with uniquely assigning the namespace at this level.

##Registering your Namespace Identifier

Please contact the Declared Registrant of the urn:nzl:pri: namespace below to register additional identifier namespaces:
 NZ Farm Data Standards
 New Zealand
 Use our [Contact page](http://www.farmdatastandards.org.nz/contact/) to email us.
You will be required to supply your organisation contact details (address and email), proposed namespace, scope of identifiers (entities covered), and optionally a POSIX regular expression that provides initial parsing for the identifiers.

##Structure
The identifier has a hierarchical structure as follows:
urn:nzl:pri:<nz-specifier>[:<nz-specifier defined string>]+
+ denotes one or more occurrences of nz-specifier defined strings all delimited by a colon.
For example:
* **urn:nzl:pri:herd:TBfree:**	    	(e.g. 4071234)
* **urn:nzl:pri:herd:NAIT:**	        (e.g. 50812345)
* **urn:nzl:pri:animal:NAIT_Traka:**	(e.g. 982-000356154301-9999999)
* **urn:nzl:pri:animal:NAIT_Visual:** (e.g. 655123-13-258974)

The <nz-specifier> and <nz-specifier defined string> can comprise any UTF-8 characters compliant with URI syntax and must not contain the ":" character (see STD 66, RFC 3986 [2]).  The exclusion of the colon from the list of other characters means that the colon can only occur as a delimiter between string values.
