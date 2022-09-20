# WORKFLOW-UNISTORE

Part of the [WORKFLOW-RS](https://github.com/workflow-rs) application framework.

***

A simple file I/O abstraction that supports browser localstorage.

Platforms supported: Native, WASM (browser)

# Features:

* A single set of per-operating-system filename configuration options with fallbacks. (i.e. filename for `macos` or `linux` will fallback on `unix` or `generic` if not defined)
* Automatic resolution of user home-folder is using `~` as a path prefix.
* Support for in-browser storage using localstorage and base64 encoding for binary data.


This crate allows you to create a single file reference while specifying multiple per-operating-system file paths, including in-browser localstorage keyname.  Subsequent read/write operations will work against the specified paths.
