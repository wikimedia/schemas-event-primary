### Version 1.1.0
- Create a local `definitions` to DRY up referencing
  repeated fields, e.g. `revision_count`.

- Declare `revision_count` field in extended page entities directly in this schema.
  `revision_count` has been removed from fragment/mediawiki/state/entity/page
  to make that entity schema more reusable.

- Add new `page.redirect_page_link` field using fragment/mediawiki/state/entity/page_link
  to represent the page to which a redirect page links to.
  https://phabricator.wikimedia.org/T325315


