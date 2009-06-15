= CREDITS =

 * initial plugin version was r1876
   * http://plugins-dev.bbpress.org/changeset/1876

= NEW NEW NEW =

 * requires HTTP_Request2
   * pear install HTTP_Request2
   * make sure that PEAR is in the include_path
   
  * requires Net_URL2
   * included as depency in HTTP_Request2
   * pear install Net_URL2
   
  * request improvements
   * only done once per request (vs. a gazillion times)
   * data is "cached" in static variables
  
  * rails api URL endpoint may require basic auth
   * add username and password to URL
   * e.g. http://foo:bar@rails.app/whatever