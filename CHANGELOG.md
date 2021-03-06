#### key

Changelog entries are classified using the following labels _(from [keep-a-changelog][]_):

- `added`: for new features
- `changed`: for changes in existing functionality
- `deprecated`: for once-stable features removed in upcoming releases
- `removed`: for deprecated features removed in this release
- `fixed`: for any bug fixes

#### [0.9.0] - 2016-07-12

**Changed**

- User-defined templates should now be stored in `~/generate/templates` instead of `~/templates`

**Added**

- [common-config][] will be used for storing user preferences. We haven't implemented any logic around this yet, but the `common-config` API is exposed on the `app.common` property, so you can begin using it in generators.


[Unreleased]: https://github.com/generate/generate/compare/0.9.0...HEAD
[0.9.0]: https://github.com/generate/generate/compare/0.8.0...0.9.0

[keep-a-changelog]: https://github.com/olivierlacan/keep-a-changelog
[common-config]: https://github.com/jonschlinkert/common-config

