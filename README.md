# Bookmarks-Wayland

- Saves bookmarks in either of 2 files "bookmarks.txt" and "bookmarks_other.txt".
- Types bookmarked links after the cursor
- Works with Wayland:
	- uses [bemenu](https://github.com/Cloudef/bemenu) as dmenu replacement
	- uses [wtype](https://github.com/atx/wtype) for typing the bookmarks

## Installation
Edit the "bookmark" file and change the location where bookmarks are saved according to your need.
Copy the file to somewhere in your PATH.

## Usage
You can run it directly from the command line but it would be most useful when you bind the various commands to various keys in your window manager. Example bindings for [Swaywm](https://swaywm.org/) are given in the file `example.sway`.

```
Usage:
bookmark [Options]

Options:
-a	Add a bookmark from the primary clipboard
-ao	Add a bookmark from the primary clipboard to the "other" bookmarks file
-s	Search and open bookmarks
-so	Search and open bookmarks from the "other" bookmarks file
-st	Search tags from both files and open the bookmark
-am	Add bookmarks by manually typing it instead of copying from clipboard
```

## Using with X11
- replace `bemenu` with `dmenu`
- replace `wtype` with `xdotool type`
