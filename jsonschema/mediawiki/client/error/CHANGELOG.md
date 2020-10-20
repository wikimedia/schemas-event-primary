### Version 1.1.0
- Use fragment/http/1.2.0, which removes client_ip (and adds protocol).
  In https://phabricator.wikimedia.org/T262626, we want to stop
  collecting client_ip by default.  eventgate-wikimedia currently uses
  the presence of the http.client_ip property in the schema to decide if
  it should set it to the value of X-Client-IP.
  This is technically a backwards incompatible change, but mediawiki/client/error
  data currently only is ingested into LogStash, which does not care.
