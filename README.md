#margi
If someone's user settings include the following, the current workspace
level formatting settings don't apply since they aren't as specific.
```
"[dart]": {
  "editor.formatOnSave": true,
  "editor.formatOnType": true,
}
```

This PR handles this by turning off auto-formatting specifically for
Dart files.

This PR also adds `"files.trimTrailingWhitespace": true` to simplify
[contribution
guide](https://github.com/flutter/flutter/wiki/Setting-up-the-Framework-development-environment#set-up-your-environment).

Fixes #122050. This change is
test-exempt.

## Pre-launch Checklist

- [x] I read the [Contributor Guide] and followed the process outlined
there for submitting PRs.
- [x] I read the [Tree Hygiene] wiki page, which explains my
responsibilities.
- [x] I read and followed the [Flutter Style Guide], including [Features
we expect every widget to implement].
- [x] I signed the [CLA].
- [x] I listed at least one issue that this PR fixes in the description
above.
- [x] I updated/added relevant documentation (doc comments with `///`).
- [x] I added new tests to check the change I am making, or this PR is
[test-exempt].
- [x] All existing and new tests are passing.
