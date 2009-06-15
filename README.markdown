# integration-api

This is a small plugin to integrate a BBPress installation with a RoR application
to provide the user with a single-sign-on across the two applications. Totally
sweet, and so on. ;-)

# changelog / readme

## CREDITS 

 * initial plugin version was r1876
   * http://plugins-dev.bbpress.org/changeset/1876

## NEW NEW NEW 

 * requires HTTP_Request2
   * (sudo) pear install HTTP_Request2
   * make sure that PEAR is in the include_path
   
 * requires Net_URL2
   * included as depency in HTTP_Request2
   * (sudo) pear install Net_URL2
   
 * request improvements
   * only done once per request (vs. a gazillion times)
   * data is "cached" in static variables
  
 * support for Basic Auth
   * RoR api URL endpoint may require Basic Auth
   * add username and password to URL
   * e.g. http://foo:bar@rails.app/whatever
   
## Feedback?

 * Patches welcome.
 * Message me (till) on github.
 * Email me: till@php.net