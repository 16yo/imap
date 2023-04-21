# My custom imap on C

Imap is a map but with integer key (id) and integer value.

Implemented on the basis of a two-way association list, the elements of which are imap_item's containing the key, value and links to the previous and next elements.

Imap is sorted by index ascending and can store multiple values with equal indices.\

One of the features of imap is that you can restore connection between chains from imap.begin and imap.back pointers if there is a gap along the way using function make_valid(imap*).
