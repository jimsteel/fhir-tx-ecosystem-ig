

### Test cases 


The tests assume that the server can accept code systems on the fly.
If servers do not accept code systems on the fly, server authors will have to 
adapt these tests by rewriting them for their own actual support code systems. 
Either way, servers that do SHOULD pass all the tests, but the FHIR product director 
will review the test outcomes in order to approve a server. 

The test cases are in version R5, but the tests will run against an R4 server. 
See [R4 and the Test Cases](r4.html)

#### Test Templates 

$$: any value

$xx$: value specifier: id, semver, url, token, string, date, version, uuid, instant, 

$optional-properties" : an array of string of properties that are allowed to be omitted

$optional$ : a boolean that can mark an object in an array as optional

$external:N$ : reference to string N in a list of external strings 

$count-array$ : ignore what's in the array, and just check the count 

$choice: array|$: a list of allowed values 

$fragments$: ??

#### Registry

{% json tests/test-cases.json liquid/test-cases.liquid %}