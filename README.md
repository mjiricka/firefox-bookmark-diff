# firefox-bookmark-diff

Python script not only for diffing two Firefox bookmark files.

I once found out that from time to time Firefox
[losts your bookmarks](http://www.tidyfavorites.com/faq/Lost%20bookmarks%20in%20Firefox.html).

In my case:
 - Some random bookmarks disappeared.
 - Some directories became empty.
 
Now I export them from time to time and compare the newly expored file
with the former one with this simple script. The script finds all empty
dirs in newer file and prints also which bookmarks were deleted (or lost)
and which were added.


## Usage

Call script with two arguments: older and newer bookmark file.

Example:

    firefox-bookmark-diff bookmarks-2015-12-22.json bookmarks-2016-01-16.json

Script will print empty directories in the second file plus compare both files.

