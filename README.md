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
* **urn:nzl:pri:herd:tbFree:**	    	(e.g. 4071234)
* **urn:nzl:pri:herd:nait:**	        (e.g. 50812345)
* **urn:nzl:pri:animal:nait_Traka:**	(e.g. 982-000356154301-9999999)
* **urn:nzl:pri:animal:nait_Visual:** (e.g. 655123-13-258974)

The <nz-specifier> and <nz-specifier defined string> can comprise any UTF-8 characters compliant with URI syntax and must not contain the ":" character (see STD 66, RFC 3986 [2]).  The exclusion of the colon from the list of other characters means that the colon can only occur as a delimiter between string values.

##Rules for Lexical Equivalence
The lexical equivalence of the NZL namespace-specific strings (NSSs) is defined as an exact, but not case-sensitive, string match.  Best Practice guidelines specify:
* NZL in either uppercase or lowercase (Names will be assigned as case-insensitive, to ensure that there will not be two NZL URNs differing only by case.)
* The first letter of each <nz-specifier> and <nz specifier defined string> in uppercase or the whole value in lowercase.
* Any identifier in NZL namespaces can be compared using the normal mechanisms for percent-encoded UTF-8 strings.
* The use of diacritic marks such as Maori macrons in identifiers is supported as described in RFC-4350.

##Sample of Existing Namespace Objects
Below are listed the existing Namespaces used primarily for the Animal Data Standards and DataLinker. Note that the processor URN is also included. There are further URN’s for each individual animal data standard attribute, which can be viewed in GitHub.
Further classes can be proposed to the Declared Registrant of the urn:nzl:pri:namespace (contact details above). It is expected, for example, that plant specific classes may be added.


* **urn:nzl:pri:animal:identity** - The Animal Identity object is comprised of the ID, the ID state, and the start and end date of the ID.

* **urn:nzl:pri:animal:loc** - The Animal Location object is comprised of the Location, the Location state, and the start and end date of the Location.

* **urn:nzl:pri:animal:herd** - The Animal Identity object is comprised of the ID, the ID state, and the start and end date of the ID.

* **urn:nzl:pri:animal:life** - The Animal Life schema is comprised of the life data of an animal, including birth date, fate, sex, species, and breed.

* **urn:nzl:pri:animal:state** - The Animal State schema describes the state of an animal, including current location, fate, fertility status, and withholding periods. 

* **urn:nzl:pri:animal:parent** - The Animal Parentage schema describes the parentage details of an animal, including parent type, birth dam ID, and sire ID.

* **urn:nzl:pri:animal:merit:herd** - The Animal Traits schema describes the breeding and index values of an animal, as identified through a genetic or derived analysis. The required fields for the traits schema include the Animal ID, bv code (or index code), and value.

* **urn:nzl:pri:animal:merit:analysis** - The merit analysis object consists of the number, date, and name of the merit value being analysed.

* **urn:nzl:pri:animal:merit:value** - The merit value object includes the relevant details for recorded a merit value such as breeding or production index values. Included are the short and full name of the merit, value, accuracy, code, and merit definition.

* **urn:nzl:pri:animal:session** - Sessions define a set of observations, or animals with observations recorded,  e.g. a session of condition scoring events.

* **urn:nzl:pri:animal:session:animal** - The session animal object defines the individual animal recorded in the session.

* **urn:nzl:pri:animal:observ** - This object describes the definitions for individual observations or traits of a group or animal.

* **urn:nzl:pri:animal:observ:cat** - This object defines the date and category of the observation recorded.

* **urn:nzl:pri:animal:observ:move** - This schema describes the movement observations of a group or animal,  including grouplID, fateCode, and disposalMethod.

* **urn:nzl:pri:animal:observ:feedgrowth** - This schema describes the feed and growth observations of a group or animal,  including grouplID, weight, and measurementType.

* **urn:nzl:pri:animal:observ:repro** - This schema describes the reproduction observations of a group or animal,  including grouplID, matingMethod, and strawID.

* **urn:nzl:pri:animal:observ:health** - This schema describes the health observations of a group or animal,  including grouplID, healthProduct, and SKU.

* **urn:nzl:pri:animal:observ:test** - This schema describes the test observations of a group or animal,  including grouplID, bloodTestType, and MIR.      

* **urn:nzl:pri:animal:observ:score** - This schema describes the score observations of a group or animal,  including grouplID, scoreCondition, and scoreVigour.

* **urn:nzl:pri:animal:dna:result** - This schema describes the dna result values for an animal,  including animallID, dnaProbability, and dnaSireId.

* **urn:nzl:pri:processor** - Processing plants. These are identifier codes used to describe a processing plant.
