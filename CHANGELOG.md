# 0.1.3 - 9 Feb 2014

- erase zipmap warnings (see CLJ-1302)
- Document `print-{warning,error}`
- warnings now have a cooldown period to prevent dynalint from
  generating too many.
  - reset `warning-interval` to configure this time, defaults to 1 second
    between warnings
- Stack traces for warnings and errors are much prettier
  - dynalint wrappers are sneakily converted to their var counterparts
    so dynalint is mostly invisible
- configure global options with `configure-linting!`
- `dynalint.lint/lint` takes the same options as `configure-linting!`

# 0.1.2 - 1 Feb 2014

- `print-{warning,error}` now accept zero arguments to print the latest error/warning
- add `zipmap` warnings that complain on directly passing the results of keys/vals
  to zipmap
- add checking for `deref`

# 0.1.1 - 12 Jan 2014

- Add ::id ex-data to warnings

# 0.1.0 - 11 Jan 2014

Initial version
