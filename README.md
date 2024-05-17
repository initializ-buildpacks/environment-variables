# `https://hub.docker.com/r/environment-variables`

Welcome to the Initializ Buildpack for Environment Variables! This nifty Cloud Native Buildpack seamlessly integrates environment variables into your image.

## Behavior

Now, let's dive into what this buildpack does when it joins the party:

* It's all about those env vars! When any environment variable matching `$BPE_*` is set, this buildpack jumps into action.

## Configuration

Alright, let's get into the nitty-gritty of configuring this buildpack:

| Environment Variable   | Description                                                |
| ---------------------- | ---------------------------------------------------------- |
| `$BPE_<NAME>`          | Sets `$NAME` to a specific value (think of it as overriding) |
| `$BPE_APPEND_<NAME>`   | Appends a value to `$NAME`                                  |
| `$BPE_DEFAULT_<NAME>`  | Sets a default value for `$NAME`                            |
| `$BPE_DELIM_<NAME>`    | Defines a delimiter to use when appending or prepending to `$NAME` |
| `$BPE_OVERRIDE_<NAME>` | Overrides `$NAME` with a specific value                    |
| `$BPE_PREPEND_<NAME>`  | Prepends a value to `$NAME`                                 |

By the way, the default delimiter is an empty string. No strings attached!

## License

This buildpack operates under version 2.0 of the [Apache License][a].
