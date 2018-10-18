### Go fmt Introduction

gofmt (read Go format) is Go's absolutly most powerful feature, this is even more a culture than a feature but its hard integration with Go and its community effecitvly qualifies it as a feature


gofmt help text:
```
-d
	Do not print reformatted sources to standard output.
	If a file's formatting is different than gofmt's, print diffs
	to standard output.
-e
	Print all (including spurious) errors.
-l
	Do not print reformatted sources to standard output.
	If a file's formatting is different from gofmt's, print its name
	to standard output.
-r rule
	Apply the rewrite rule to the source before reformatting.
-s
	Try to simplify code (after applying the rewrite rule, if any).
-w
	Do not print reformatted sources to standard output.
	If a file's formatting is different from gofmt's, overwrite it
	with gofmt's version. If an error occurred during overwriting,
	the original file is restored from an automatic backup.
```

Every odd file represents a malformat file and every following even file represents the output of `gofmt -w`, basically applying the Go Format
