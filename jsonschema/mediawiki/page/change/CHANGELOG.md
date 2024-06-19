### Version 1.2.0
- performer is now optional by using fragment/mediawiki/state/change/1.2.0.
  We don't set performer for revision visibility changes where the change is
  admin suppressed.
  https://phabricator.wikimedia.org/T342487
  NOTE: While removing required-ness is technically a breaking change
  that requires a major version bump,
  it should not break any consumers in this case.
  We've added an exception in .jsonschema-tools.yaml to skip the
  backwards compatibility check for version 1.2.0.
