# Dart Format `pre-commit`

[`https://pre-commit.com`](https://pre-commit.com) hook for formatting Dart files.

Add the following in your `.pre-commit-config.yaml`:
```yaml
- repo: https://github.com/Cretezy/dart-format-pre-commit
  rev: "master"
  hooks:
    - id: dart-format
```

You can also only include/exclude some files (defaults to only `.dart`, is a pattern):

```yaml
- repo: https://github.com/Cretezy/dart-format-pre-commit
  rev: "master"
  hooks:
    - id: dart-format
      files: lib/* # Only format source files
      exclude: lib/src/utils.dart # Exclude utils
```

## Flutter

Also see [Flutter Format `pre-commit`](https://github.com/Cretezy/flutter-format-pre-commit) for formatting Flutter code.
