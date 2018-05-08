# Changelog

This file contains the changes made for each version of `nbinteract`. Since
the package contains both a Python and a JavaScript component, we keep the
version numbers for both Python and JS packages the same so updates are easier
to keep track of.

## master

## 0.1.8

**JS**

Bug fixes:

- Fixes nbinteract-core loading on unpkg.

## 0.1.7

**Python**

Bug fixes:

- Ensures template files are included in package

## 0.1.6

**Python**

Features:

- Add `--execute` flag to CLI that correctly generates widget output.

Bug fixes:

- Fixes CLI `--output` flag for Python 3.4

**JS**

Features:

- Errors in widget code get displayed in the status buttons.

## 0.1.5

**Python**

Bug fixes:

- Fixes error when some plotting functions are called.

## 0.1.4

**Python**

Features:

- `nbinteract init` initializes a GitHub repo for nbinteract.

**JS**

Bug fixes:

- Fixes errors from cells that don't have widget output.

## 0.1.3

**Python**

Features:

- The `nbinteract` CLI now has a `--no-top-button` flag to remove the top-level
  button.

Bug fixes:

- Python 3.4 doesn't support the `{**dict1, **dict2}` syntax, so we merge
  dictionaries another way to support older versions of Python.
- Fixes an issue that broke `nbinteract` CLI completely (#52).
- The `nbinteract` CLI spec argument didn't actually set the spec properly.

**JS**

Bug fixes:

- Fixes `nbinteract-core` so that loading it in a webpage initializes the
  NbInteract variable properly.

## 0.1.2

**Python**

Changes:

- `nbi.publish()` and the `nbinteract` CLI tool now require a Binder spec as
  input.

Features:

- `nbi.publish()` and the `nbinteract` CLI tool now allow for template
  selection.
- The `nbinteract` CLI tool gets a major overhaul with options to recurse into
  subdirectories and output files in specified folders.

**JS**

Bug fixes:

- Fixed an issue where lots of error message were getting logged to the console
  in the GitBook (https://github.com/SamLau95/nbinteract/issues/41).

## 0.1.1

**Python**

Bugs fixed:

- Converting using `full.tpl` now correctly cells with `# HIDDEN`
  (https://github.com/SamLau95/nbinteract/pull/43/)
- Using `nbi.publish` now works on Python versions < 3.5
  (https://github.com/SamLau95/nbinteract/pull/43/)
