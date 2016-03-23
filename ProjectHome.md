
---

# The Project has been moved to http://www.badgenow.com/p/radixtree #

---



A radix tree, Patricia trie/tree, or crit bit tree is a specialized set data structure based on the trie that is used to store a set of strings. In contrast with a regular trie, the edges of a Patricia trie are labelled with sequences of characters rather than with single characters. These can be strings of characters, bit strings such as integers or IP addresses, or generally arbitrary sequences of objects in lexicographical order. Sometimes the names radix tree and crit bit tree are only applied to trees storing integers and Patricia trie is retained for more general inputs, but the structure works the same way in all cases.

For more information see http://en.wikipedia.org/wiki/Radix_tree

I have created this Radix tree for a project that required fast searching of user name prefixes for a Google AJAX Search like interface.

Radix Tree gives fastest possible ways to search prefixes. For example it can quickly answer queries like "Find all user name starting with 'tahseen'"

The database solution for this problem boils down to queries like
`select * from user where username like 'tahseen%'`

Database solution does not scale very well if you have a large number of concurrent users searching.

A memory based Radix Tree scale very well.

**Update: (1st Sept 2009)** A new method added that would complete a given string to the point where the ambiguity starts. (Contribution by kaljurand (http://code.google.com/u/kaljurand/))

**Update: (23rd June 2009)** Dennis Heidsiek <HeidsiekB at aol dot com> improvements has been merged with trunk.

**Update:** Javid Jamae (http://www.javidjamae.com/) has provided an excellent implementation of Radix tree in javascript. Go ahead and download it!