EXPLANATION

INITIALIZATION When a new Node is created, it\'s previous and next
pointers are set to None, since it\'s not connected to other nodes.
Similarly,for the new DLL instance,head is set to None,since the list is
empty.

INSERTION a)at begining A new node(n) inseted with given data. If list
is empty,set head to the n. Else: First,set the n.next to the current
head and current head\'s prev to the n,finally,update head to n.

b)at end A new node(n) inseted with given data. If the list is empty,set
head to the n. Else: First,traverse list to find k and set the last
node.next to the n and finally,set n.prev to the last node. c)at
specific position Insert i_beg at the beginning and create a new
node(n). Traverse to reach node before specific position.If traversal is
None before specific position,then use IndexError. Adjusting pointers by
setting n.next to the current node\'s next.If the current node\'s next
exists, set prev to n and set the current node\'s next to the n and
finally,set the n.prev to the current node.

DELETION a)at begining If list is empty,print a message. If Only One
Node Exists,Set head to None, making the list empty. If Multiple Nodes
exists,first,Update head to point to the second node,then,Set the new
head\'s prev to None. b)at end If list is empty,print a message. If Only
One Node Exists,Set head to None, making the list empty. If Multiple
Nodes exist,first,Traverse to the last node (k),then,Set the second last
node\'s next to None, effectively removing the last node. c)at specific
position If list is empty,print a message and exit Function d_beg is
used to delete from the beginning. If traversal reaches None before
specific position, then use IndexError. If the node to be deleted is the
last node,set current node\'s next to None,else,set the current node\'s
next to skip the node to be deleted and point to the n,and finally ,set
the n.prev to the current node.

TRAVESAL a)forward If list is empty,print a message. Else: Starting with
head,go through each node. Print each node\'s data. Print a new line
after traversal. b)backward If list is empty,print a message. Elif (to
the end): Starting with head,go through each node until last. Else: From
the last node, go backward ,then,print each node\'s data followed by a
space. print a new line after traversal.

\"\"\"
