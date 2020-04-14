'Primary' event JSONSchemas for Wikimedia & Mediawiki event data.

This schema repository contains event schemas that directly affect
use facing features.  These schemas are meant to represent 'tier 1' events.
This resository compliments the [schemas/event/secondary](https://gerrit.wikimedia.org/r/plugins/gitiles/schemas/event/secondary/+/master) repository.

See also:
- (Event Platform/Schemas)[https://wikitech.wikimedia.org/wiki/Event_Platform/Schemas]
- (Event Platform/Schemas/Guidelines)[https://wikitech.wikimedia.org/wiki/Event_Platform/Schemas/Guidelines]


NOTE: The only reason for having separate event schema repositories is to
allow for different repository merge rights.  Changes to primary schemas need
to be more restricted than changes to secondary schemas.
