# Builtins

Source: ITPIE:OPS Documentation — Builtins
Source URL: https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Builtins
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] This document describes the various built-in functions available in scriban.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Array functions available through the object 'array' in scriban.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.add
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.add_range
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.compact
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.concat
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.cycle
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.each
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.filter
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.first
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.insert_at
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.join
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.last
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.limit
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.map
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.offset
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.remove_at
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.reverse
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.size
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.sort
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.uniq
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.contains
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.add
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.add <list> <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds a value to the input list.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The value to add at the end of the list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new list with the value added
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, 2, 3] | array.add 4 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [1, 2, 3, 4]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.add_range
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.add_range <list1> <list2>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Concatenates two lists.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list1 : The 1st input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list2 : The 2nd input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The concatenation of the two input lists
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, 2, 3] | array.add_range [4, 5] }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [1, 2, 3, 4, 5]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.compact
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.compact <list>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes any null values from the input list.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : An input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a list with null value removed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, null, 3] | array.compact }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [1, 3]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.concat
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.concat <list1> <list2>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Concatenates two lists.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list1 : The 1st input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list2 : The 2nd input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The concatenation of the two input lists
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, 2, 3] | array.concat [4, 5] }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [1, 2, 3, 4, 5]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.cycle
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.cycle <list> <group>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Loops through a group of strings and outputs them in the order that they were passed as parameters. Each time cycle is called, the next string that was passed as a parameter is output.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : An input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] group : The group used. Default is null
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a list with null value removed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ array.cycle ['one', 'two', 'three'] }} {{ array.cycle ['one', 'two', 'three'] }} {{ array.cycle ['one', 'two', 'three'] }} {{ array.cycle ['one', 'two', 'three'] }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] one two three one
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] cycle accepts a parameter called cycle group in cases where you need multiple cycle blocks in one template. If no name is supplied for the cycle group, then it is assumed that multiple calls with the same parameters are one group.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.each
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.each <list> <function>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Applies the specified function to each element of the input.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : An input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] function : The function to apply to each item in the list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a list with each item being transformed by the function.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [" a", " 5", "6 "] | array.each @string.strip }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["a", "5", "6"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.filter
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.filter <list> <function>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Filters the input list according the supplied filter function.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : An input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] function : The function used to test each elemement of the list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a new list which contains only those elements which match the filter function.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{["", "200", "","400"] | array.filter @string.empty}}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["", ""]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.first
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.first <list>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the first element of the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The first element of the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6] | array.first }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.insert_at
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.insert_at <list> <index> <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Inserts a value at the specified index in the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] index : The index in the list where to insert the element
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The value to insert
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new list with the element inserted.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ ["a", "b", "c"] | array.insert_at 2 "Yo" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["a", "b", "Yo", "c"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.join
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.join <list> <delimiter> <function>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Joins the element of a list separated by a delimiter string and return the concatenated string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] delimiter : The delimiter string to use to separate elements in the output string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] function : An optional function that will receive the string representation of the item to join and can transform the text before joining.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new list with the element inserted.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, 2, 3] | array.join "|" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 1|2|3
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.last
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.last <list>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the last element of the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The last element of the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6] | array.last }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.limit
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.limit <list> <count>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a limited number of elments from the input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] count : The number of elements to return from the input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6] | array.limit 2 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [4, 5]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.map
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.map <list> <member>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Accepts an array element's attribute as a parameter and creates an array out of each array element's value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] member : The member to extract the value from
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ products = [{title: "orange", type: "fruit"}, {title: "computer", type: "electronics"}, {title: "sofa", type: "furniture"}] products | array.map "type" | array.uniq | array.sort }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["electronics", "fruit", "furniture"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.offset
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.offset <list> <index>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the remaining of the list after the specified offset
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] index : The index of a list to return elements
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6, 7, 8] | array.offset 2 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [6, 7, 8]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.remove_at
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.remove_at <list> <index>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes an element at the specified index from the input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] index : The index of a list to return elements
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new list with the element removed. If index is negative, remove at the end of the list.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6, 7, 8] | array.remove_at 2 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [4, 5, 7, 8]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] If the index is negative, removes at the end of the list (notice that we need to put -1 in parenthesis to avoid confusing the parser with a binary - operation):
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6, 7, 8] | array.remove_at (-1) }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [4, 5, 6, 7]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.reverse
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.reverse <list>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Reverses the input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new list in reversed order.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6, 7] | array.reverse }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [7, 6, 5, 4]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.size
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.size <list>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the number of elements in the input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A number of elements in the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [4, 5, 6] | array.size }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.sort
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.sort <list> <member>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Sorts the elements of the input list according to the value of each element or the value of the specified member of each element
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] member : The member name to sort according to its value. Null by default, meaning that the element's value are used instead.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A list sorted according to the value of each element or the value of the specified member of each element.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Sorts by element's value:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [10, 2, 6] | array.sort }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [2, 6, 10]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Sorts by elements member's value:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ products = [{title: "orange", type: "fruit"}, {title: "computer", type: "electronics"}, {title: "sofa", type: "furniture"}] products | array.sort "title" | array.map "title" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["computer", "orange", "sofa"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.uniq
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.uniq <list>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the unique elements of the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A list of unique elements of the input list .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, 1, 4, 5, 8, 8] | array.uniq }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [1, 4, 5, 8]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.contains
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] array.contains <list> <item>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns if a list contains a specific item .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] list : The input list
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] item : The input item
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true if item is in list ; otherwise false
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, 2, 3, 4] | array.contains 4 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A datetime object represents an instant in time, expressed as a date and time of day.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Name Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .year Gets the year of a date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .month Gets the month of a date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .day Gets the day in the month of a date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .day_of_year Gets the day within the year
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .hour Gets the hour of the date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .minute Gets the minute of the date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .second Gets the second of the date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .millisecond Gets the millisecond of the date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Binary operations
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The subtract operation date1 - date2 : Subtract date2 from date1 and return a timespan internal object (see timespan object below).
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Other comparison operators( == , != , <= , >= , < , > ) are also working with date objects.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan and also the added to a datetime object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.now
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_days
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_months
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_years
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_hours
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_minutes
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_seconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_milliseconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.parse
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.to_string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.now
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a datetime object of the current time, including the hour, minutes, seconds and milliseconds.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ date.now.year }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 2024
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_days
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_days <date> <days>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds the specified number of days to the input date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date : The date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] days : The days.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ date.parse '2016/01/05' | date.add_days 1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 06 Jan 2016
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_months
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_months <date> <months>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds the specified number of months to the input date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date : The date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] months : The months.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ date.parse '2016/01/05' | date.add_months 1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 05 Feb 2016
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_years
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_years <date> <years>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds the specified number of years to the input date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date : The date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] years : The years.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ date.parse '2016/01/05' | date.add_years 1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 05 Jan 2017
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_hours
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_hours <date> <hours>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds the specified number of hours to the input date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date : The date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] hours : The hours.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_minutes
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_minutes <date> <minutes>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds the specified number of minutes to the input date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date : The date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] minutes : The minutes.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_seconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_seconds <date> <seconds>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds the specified number of seconds to the input date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date : The date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] seconds : The seconds.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_milliseconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.add_milliseconds <date> <millis>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Adds the specified number of milliseconds to the input date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date : The date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] millis : The milliseconds.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.parse
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.parse <text> <pattern>? <culture>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Parses the specified input string to a date object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : A text representing a date.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The date format pattern. See to_string method about the format of a pattern.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] culture : The culture used to format the datetime. Default is current culture.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A date object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ date.parse '2016/01/05' }} {{ date.parse '2018--06--17' '%Y--%m--%d' }} {{ date.parse '2021/11/30 20:50:23Z' }} {{ date.parse '20/01/2022 08:32:48 +00:00' culture:'en-GB' }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 05 Jan 2016 17 Jun 2018 30 Nov 2021 20 Jan 2022
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.to_string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] date.to_string <datetime> <pattern> <culture>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a datetime object to a textual representation using the specified format string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] By default, if you are using a date, it will use the format specified by date.format which defaults to date.default_format (readonly) which default to %d %b %Y
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] You can override the format used for formatting all dates by assigning the a new format: date.format = '%a %b %e %T %Y';
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] You can recover the default format by using date.format = date.default_format;
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] By default, the to_string format is using the current culture , but you can switch to an invariant culture by using the modifier %g
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] For example, using %g %d %b %Y will output the date using an invariant culture.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] If you are using %g alone, it will output the date with date.format using an invariant culture.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Suppose that date.now would return the date 2013-09-12 22:49:27 +0530 , the following table explains the format modifiers:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Format Result Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%a" "Thu" Name of week day in short form of the
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%A" "Thursday" Week day in full form of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%b" "Sep" Month in short form of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%B" "September" Month in full form of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%c" Date and time (%a %b %e %T %Y)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%C" "20" Century of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%d" "12" Day of the month of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%D" "09/12/13" Date (%m/%d/%y)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%e" "12" Day of the month, blank-padded ( 1..31)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%F" "2013-09-12" ISO 8601 date (%Y-%m-%d)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%h" "Sep" Alias for %b
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%H" "22" Hour of the time in 24 hour clock format
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%I" "10" Hour of the time in 12 hour clock format
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%j" "255" Day of the year (001..366) (3 digits, left padded with zero)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%k" "22" Hour of the time in 24 hour clock format, blank-padded ( 0..23)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%l" "10" Hour of the time in 12 hour clock format, blank-padded ( 0..12)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%L" "000" Millisecond of the time (3 digits, left padded with zero)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%m" "09" Month of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%M" "49" Minutes of the time (2 digits, left padded with zero e.g 01 02)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%n" Newline character (\n)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%N" "000000000" Nanoseconds of the time (9 digits, left padded with zero)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%p" "PM" Gives AM / PM of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%P" "pm" Gives am / pm of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%r" "10:49:27 PM" Long time in 12 hour clock format (%I:%M:%S %p)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%R" "22:49" Short time in 24 hour clock format (%H:%M)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%s" Number of seconds since 1970-01-01 00:00:00 +0000
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%S" "27" Seconds of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%t" Tab character (\t)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%T" "22:49:27" Long time in 24 hour clock format (%H:%M:%S)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%u" "4" Day of week of the time (from 1 for Monday to 7 for Sunday)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%U" "36" Week number of the current year, starting with the first Sunday as the first day of the first week (00..53)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%v" "12-SEP-2013" VMS date (%e-%b-%Y) (culture invariant)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%V" "37" Week number of the current year according to ISO 8601 (01..53)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%W" "36" Week number of the current year, starting with the first Monday as the first day of the first week (00..53)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%w" "4" Day of week of the time (from 0 for Sunday to 6 for Saturday)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%x" Preferred representation for the date alone, no time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%X" Preferred representation for the time alone, no date
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%y" "13" Gives year without century of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%Y" "2013" Year of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%Z" "+05:30" Gives Time Zone of the time
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "%%" "%" Output the character %
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Note that the format is using a good part of the ruby format ( source )
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ date.parse '2016/01/05' | date.to_string '%d %b %Y' }} {{ date.parse '2016/01/05' | date.to_string '%d %B %Y' 'fr-FR' }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 05 Jan 2016 05 janvier 2016
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] datetime : The input datetime to format
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The date format pattern.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] culture : The culture used to format the datetime
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A that represents this instance.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Html functions available through the builtin object 'html'.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.strip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.url_encode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.url_escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.strip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.strip <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes any HTML tags from the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string removed with any HTML tags
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Notice that the implementation of this function is using a simple regex, so it can fail escaping correctly or timeout in case of the malformed html. If you are looking for a secure HTML stripped, you might want to plug your own HTML function by using AngleSharp to strip these HTML tags.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "<p>This is a paragraph</p>" | html.strip }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] This is a paragraph
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.escape <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Escapes a HTML input string (replacing & by &amp; )
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string removed with any HTML tags
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "<p>This is a paragraph</p>" | html.escape }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] &lt;p&gt;This is a paragraph&lt;/p&gt;
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.url_encode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.url_encode <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts any URL-unsafe characters in a string into percent-encoded characters.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string url encoded
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "john@liquid.com" | html.url_encode }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] john%40liquid.com
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.url_escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] html.url_escape <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Identifies all characters in a string that are not allowed in URLS, and replaces the characters with their escaped variants.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string url escaped
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "<hello> & <scriban>" | html.url_escape }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] %3Chello%3E%20&%20%3Cscriban%3E
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Math functions available through the object 'math' in scriban.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.abs
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.ceil
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.divided_by
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.floor
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.format
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.is_number
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.minus
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.modulo
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.plus
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.round
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.times
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.uuid
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.random
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.abs
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.abs <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the absolute value of a specified number.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The absolute value of the input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ -15.5| math.abs }} {{ -5| math.abs }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 15.5 5
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.ceil
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.ceil <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the smallest integer greater than or equal to the specified number.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The smallest integer greater than or equal to the specified number.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 4.6 | math.ceil }} {{ 4.3 | math.ceil }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 5 5
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.divided_by
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.divided_by <value> <divisor>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Divides the specified value by another value. If the divisor is an integer, the result will be floor to and converted back to an integer.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] divisor : The divisor value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The division of value by divisor .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 8.4 | math.divided_by 2.0 | math.round 1 }} {{ 8.4 | math.divided_by 2 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 4.2 4
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.floor
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.floor <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the largest integer less than or equal to the specified number.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The largest integer less than or equal to the specified number.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 4.6 | math.floor }} {{ 4.3 | math.floor }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 4 4
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.format
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.format <value> <format> <culture>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Formats a number value with specified .NET standard numeric format strings
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] format : The format string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] culture : The culture as a string (e.g en-US ). By default the culture from is used
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The largest integer less than or equal to the specified number.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 255 | math.format "X4" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 00FF
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.is_number
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.is_number <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a boolean indicating if the input value is a number
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true if the input value is a number; otherwise false.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 255 | math.is_number }} {{ "yo" | math.is_number }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true false
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.minus
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.minus <value> <with>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Subtracts from the input value the with value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] with : The with value to subtract from value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The results of the subtraction: value - with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 255 | math.minus 5}}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 250
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.modulo
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.modulo <value> <with>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Performs the modulo of the input value with the with value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] with : The with value to module value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The results of the modulo: value % with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 11 | math.modulo 10}}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.plus
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.plus <value> <with>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Performs the addition of the input value with the with value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] with : The with value to add to value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The results of the addition: value + with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 1 | math.plus 2}}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.round
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.round <value> <precision: 0>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Rounds a value to the nearest integer or to the specified number of fractional digits.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] precision : The number of fractional digits in the return value. Default is 0.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A value rounded to the nearest integer or to the specified number of fractional digits.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 4.6 | math.round }} {{ 4.3 | math.round }} {{ 4.5612 | math.round 2 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 5 4 4.56
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.times
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.times <value> <with>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Performs the multiplication of the input value with the with value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] with : The with value to multiply to value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The results of the multiplication: value * with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 2 | math.times 3}}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.uuid
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Creates a new UUID
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The created UUID, ex. 2dc55d50-3f6c-446a-87d0-a5a4eed23269
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ math.uuid }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 1c0a4aa8-680e-4bd6-95e9-cdbec45ef057
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.random
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] math.random <minValue> <maxValue>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Creates a random number
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] minValue : The inclusive lower bound of the random number returned
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] maxValue : The exclusive upper bound of the random number returned. maxValue must be greater than or equal to minValue.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A random number greater or equal to minValue and less than maxValue
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ math.random 1 10 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Object functions available through the builtin object 'object'.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.default
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.eval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.eval_template
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.format
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.has_key
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.has_value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.keys
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.size
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.typeof
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.kind
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.values
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.from_json
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.to_json
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.default
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.default <value> <default>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The default value is returned if the input value is null or an empty string "". A string containing whitespace characters will not resolve to the default value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value to check if it is null or an empty string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] default : The default value to return if the input value is null or an empty string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The default value is returned if the input value is null or an empty string "", otherwise it returns value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ undefined_var | object.default "Yo" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.eval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.eval <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The evaluates a string as a scriban expression or evaluate the passed function or return the passed value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value, either a scriban template in a string, or an alias function or directly a value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The evaluation of the input value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "1 + 2" | object.eval }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.eval_template
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.eval_template <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The evaluates a string as a scriban template or evaluate the passed function or return the passed value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value, either a scriban template in a string, or an alias function or directly a value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The evaluation of the input value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "This is a template text {{ 1 + 2 }}" | object.eval_template }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] This is a template text 3
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.format
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.format <value> <format> <culture>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Formats an object using specified format.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] format : The format string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] culture : The culture as a string (e.g en-US ). By default the culture from is used
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 255 | object.format "X4" }} {{ 1523 | object.format "N2" "en-US" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 00FF 1,523.00
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.has_key
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.has_key <value> <key>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Checks if the specified object as the member key
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] key : The member name to check its existence.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true if the input object contains the member key ; otherwise false
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ product | object.has_key "title" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.has_value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.has_value <value> <key>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Checks if the specified object as a value for the member key
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] key : The member name to check the existence of its value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true if the input object contains the member key and has a value; otherwise false
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ product | object.has_value "title" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.keys
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.keys <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Gets the members/keys of the specified value object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A list with the member names/key of the input object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ product | object.keys | array.sort }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["title", "type"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.size
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.size <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the size of the input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] If the input object is a string, it will return the length
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] If the input is a list, it will return the number of elements
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] If the input is an object, it will return the number of members
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The size of the input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ [1, 2, 3] | object.size }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.typeof
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.typeof <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns string representing the type of the input object. The type can be string , boolean , number , array , iterator and object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ null | object.typeof }} {{ true | object.typeof }} {{ 1 | object.typeof }} {{ 1.0 | object.typeof }} {{ "text" | object.typeof }} {{ 1..5 | object.typeof }} {{ [1,2,3,4,5] | object.typeof }} {{ {} | object.typeof }} {{ object | object.typeof }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] boolean number number string iterator array object object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.kind
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.kind <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns string representing the type of the input object. The type can be string , bool , byte , sbyte , ushort , short , uint , int , ulong , long , float , double , decimal , bigint , enum , range , array , function and object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] This function is newer than object.typeof and returns more detailed results about the types (e.g instead of number , returns int or double )
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ null | object.kind }} {{ true | object.kind }} {{ 1 | object.kind }} {{ 1.0 | object.kind }} {{ "text" | object.kind }} {{ 1..5 | object.kind }} {{ [1,2,3,4,5] | object.kind }} {{ {} | object.kind }} {{ object | object.kind }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] bool int double string range array object object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.values
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.values <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Gets the member's values of the specified value object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A list with the member values of the input object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ product | object.values | array.sort }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["fruit", "Orange"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.from_json
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.from_json <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a JSON string to a scriban value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input JSON string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The scriban value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ obj = `{ "foo": 123 }` | object.from_json obj.foo }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 123
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.to_json
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] object.to_json <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a scriban value to a JSON string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The input value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A JSON representation of the value.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ { foo: "bar", baz: [1, 2, 3] } | object.to_json }} {{ true | object.to_json }} {{ null | object.to_json }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {"foo":"bar","baz":[1,2,3]} true null
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Functions exposed through regex builtin object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Note: If your regular expression contains backslashes ( \ ), you will need to do one of the following:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Anywhere you would use a \ , use two. For example: "\d+\.\d+" becomes "\\d+\\.\\d+"
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Use verbatim strings . For example: "\d+\.\d+" becomes `\d+\.\d+`
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.match
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.matches
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.replace
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.split
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.unescape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.escape <pattern>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Escapes a minimal set of characters ( \ , * , + , ? , | , { , [ , ( , ) , ^ , $ , . , # , and white space) by replacing them with their escape codes. This instructs the regular expression engine to interpret these characters literally rather than as metacharacters.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The input string that contains the text to convert.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A string of characters with metacharacters converted to their escaped form.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "(abc.*)" | regex.escape }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] \(abc\.\*\)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.match
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.match <text> <pattern> <options>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Searches an input string for a substring that matches a regular expression pattern and returns an array with the match occurences.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to search for a match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The regular expression pattern to match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] options : A string with regex options, that can contain the following option characters (default is null ):
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] i : Specifies case-insensitive matching.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] m : Multiline mode. Changes the meaning of ^ and $ so they match at the beginning and end, respectively, of any line, and not just the beginning and end of the entire string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] s : Specifies single-line mode. Changes the meaning of the dot . so it matches every character (instead of every character except \n ).
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] x : Eliminates unescaped white space from the pattern and enables comments marked with # .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] An array that contains all the match groups. The first group contains the entire match. The other elements contain regex matched groups (..) . An empty array returned means no match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "this is a text123" | regex.match `(\w+) a ([a-z]+\d+)` }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["is a text123", "is", "text123"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Notice that the first element returned in the array is the entire regex match, followed by the regex group matches.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.matches
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.matches <text> <pattern> <options>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Searches an input string for multiple substrings that matches a regular expression pattern and returns an array with the match occurences.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to search for a match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The regular expression pattern to match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] options : A string with regex options, that can contain the following option characters (default is null ):
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] i : Specifies case-insensitive matching.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] m : Multiline mode. Changes the meaning of ^ and $ so they match at the beginning and end, respectively, of any line, and not just the beginning and end of the entire string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] s : Specifies single-line mode. Changes the meaning of the dot . so it matches every character (instead of every character except \n ).
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] x : Eliminates unescaped white space from the pattern and enables comments marked with # .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] An array of matches that contains all the match groups. The first group contains the entire match. The other elements contain regex matched groups (..) . An empty array returned means no match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "this is a text123" | regex.matches `(\w+)` }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] [["this", "this"], ["is", "is"], ["a", "a"], ["text123", "text123"]]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Notice that the first element returned in the sub array is the entire regex match, followed by the regex group matches.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.replace
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.replace <text> <pattern> <replace> <options>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] In a specified input string, replaces strings that match a regular expression pattern with a specified replacement string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to search for a match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The regular expression pattern to match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] replace : The replacement string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] options : A string with regex options, that can contain the following option characters (default is null ):
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] i : Specifies case-insensitive matching.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] m : Multiline mode. Changes the meaning of ^ and $ so they match at the beginning and end, respectively, of any line, and not just the beginning and end of the entire string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] s : Specifies single-line mode. Changes the meaning of the dot . so it matches every character (instead of every character except \n ).
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] x : Eliminates unescaped white space from the pattern and enables comments marked with # .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A new string that is identical to the input string, except that the replacement string takes the place of each matched string. If pattern is not matched in the current instance, the method returns the current instance unchanged.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "abbbbcccd" | regex.replace "b+c+" "-Yo-" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] a-Yo-d
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.split
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.split <text> <pattern> <options>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Splits an input string into an array of substrings at the positions defined by a regular expression match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to split.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The regular expression pattern to match.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] options : A string with regex options, that can contain the following option characters (default is null ):
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] i : Specifies case-insensitive matching.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] m : Multiline mode. Changes the meaning of ^ and $ so they match at the beginning and end, respectively, of any line, and not just the beginning and end of the entire string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] s : Specifies single-line mode. Changes the meaning of the dot . so it matches every character (instead of every character except \n ).
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] x : Eliminates unescaped white space from the pattern and enables comments marked with # .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A string array.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "a, b , c, d" | regex.split `\s*,\s*` }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ["a", "b", "c", "d"]
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.unescape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] regex.unescape <pattern>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts any escaped characters in the input string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] pattern : The input string containing the text to convert.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A string of characters with any escaped characters converted to their unescaped form.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "\\(abc\\.\\*\\)" | regex.unescape }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] (abc.*)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] String functions available through the builtin object 'string`.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.append
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.capitalize
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.capitalizewords
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.contains
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.empty
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.whitespace
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.downcase
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.ends_with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.equals_ignore_case
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.handleize
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.literal
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.lstrip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pluralize
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.prepend
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove_first
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove_last
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.replace
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.replace_first
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.rstrip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.size
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.slice
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.slice1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.split
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.starts_with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.strip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.strip_newlines
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_int
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_long
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_float
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_double
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.truncate
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.truncatewords
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.upcase
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.md5
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.sha1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.sha256
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.hmac_sha1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.hmac_sha256
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pad_left
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pad_right
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.base64_encode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.base64_decode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.index_of
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.escape
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.escape <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Escapes a string with escape characters.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The two strings concatenated
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Hel\tlo\n\"W\\orld" | string.escape }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hel\tlo\n\"W\\orld
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.append
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.append <text> <with>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Concatenates two strings
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] with : The text to append
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The two strings concatenated
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Hello" | string.append " World" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hello World
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.capitalize
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.capitalize <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts the first character of the passed string to a upper case character.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The capitalized input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.capitalize }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Test
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.capitalizewords
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.capitalizewords <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts the first character of each word in the passed string to a upper case character.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The capitalized input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "This is easy" | string.capitalizewords }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] This Is Easy
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.contains
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.contains <text> <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a boolean indicating whether the input string contains the specified string value .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The string to look for
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] if text contains the string value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "This is easy" | string.contains "easy" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.empty
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.empty <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a boolean indicating whether the input string is an empty string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] if text is an empty string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "" | string.empty }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.whitespace
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.whitespace <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a boolean indicating whether the input string is empty or contains only whitespace characters.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] if text is empty string or contains only whitespace characters
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "" | string.whitespace }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.downcase
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.downcase <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts the string to lower case.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string lower case
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "TeSt" | string.downcase }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] test
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.ends_with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.ends_with <text> <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a boolean indicating whether the input string ends with the specified string value .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The string to look for
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] if text ends with the specified string value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "This is easy" | string.ends_with "easy" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.equals_ignore_case
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.equals_ignore_case <text> <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a boolean indicating whether the input string is equal to specified string 'value'. Comparison is case insensitive.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The string to compare
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] if text is equal to string value , ignoring case
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Scriban" | string.equals_ignore_case "SCRIBAN" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.handleize
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.handleize <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a url handle from the input string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A url handle
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ '100% M & Ms!!!' | string.handleize }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 100-m-ms
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.literal
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.literal <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Return a string literal enclosed with double quotes of the input string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to return a literal from.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The literal of a string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] If the input string has non printable characters or they need contain a double quote, they will be escaped.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ 'Hello\n"World"' | string.literal }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] "Hello\n\"World\""
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.lstrip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.lstrip <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes any whitespace characters on the left side of the input string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string without any left whitespace characters
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ ' too many spaces' | string.lstrip }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Highlight to see the empty spaces to the right of the string output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] too many spaces
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pluralize
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pluralize <number> <singular> <plural>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Outputs the singular or plural version of a string based on the value of a number.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] number : The number to check
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] singular : The singular string to return if number is == 1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] plural : The plural string to return if number is != 1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The singular or plural string based on number
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ products.size }} {{products.size | string.pluralize 'product' 'products' }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 7 products
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.prepend
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.prepend <text> <by>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Concatenates two strings by placing the by string in from of the text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] by : The string to prepend to text
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The two strings concatenated
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "World" | string.prepend "Hello " }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hello World
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove <text> <remove>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes all occurrences of a substring from a string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] remove : The substring to remove from the text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string with the all occurence of a substring removed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Hello, world. Goodbye, world." | string.remove "world" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hello, . Goodbye, .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove_first
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove_first <text> <remove>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes the first occurrence of a substring from a string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] remove : The first occurence of substring to remove from the text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string with the first occurence of a substring removed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Hello, world. Goodbye, world." | string.remove_first "world" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hello, . Goodbye, world.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove_last
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.remove_last <text> <remove>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes the last occurrence of a substring from a string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] remove : The last occurence of substring to remove from the text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string with the first occurence of a substring removed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Hello, world. Goodbye, world." | string.remove_last "world" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hello, world. Goodbye, .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.replace
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.replace <text> <match> <replace>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Replaces all occurrences of a string with a substring.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] match : The substring to find in the text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] replace : The substring used to replace the string matched by match in the input text
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string replaced
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Hello, world. Goodbye, world." | string.replace "world" "buddy" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hello, buddy. Goodbye, buddy.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.replace_first
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.replace_first <text> <match> <replace> <fromEnd: False>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Replaces the first occurrence of a string with a substring.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] match : The substring to find in the text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] replace : The substring used to replace the string matched by match in the input text
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] fromEnd : if true start match from end
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string replaced
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "Hello, world. Goodbye, world." | string.replace_first "world" "buddy" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hello, buddy. Goodbye, world.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.rstrip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.rstrip <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes any whitespace characters on the right side of the input string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string without any left whitespace characters
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ ' too many spaces ' | string.rstrip }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Highlight to see the empty spaces to the right of the string output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] too many spaces
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.size
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.size <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns the number of characters from the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The length of the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.size }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.slice
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.slice <text> <start> <length>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The slice returns a substring, starting at the specified index. An optional second parameter can be passed to specify the length of the substring. If no second parameter is given, a substring with the remaining characters will be returned.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] start : The starting index character where the slice should start from the input text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] length : The number of character. Default is 0, meaning that the remaining of the string will be returned.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string sliced
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "hello" | string.slice 0 }} {{ "hello" | string.slice 1 }} {{ "hello" | string.slice 1 3 }} {{ "hello" | string.slice 1 length:3 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] hello ello ell ell
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.slice1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.slice1 <text> <start> <length: 1>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The slice returns a substring, starting at the specified index. An optional second parameter can be passed to specify the length of the substring. If no second parameter is given, a substring with the first character will be returned.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] start : The starting index character where the slice should start from the input text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] length : The number of character. Default is 1, meaning that only the first character at start position will be returned.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string sliced
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "hello" | string.slice1 0 }} {{ "hello" | string.slice1 1 }} {{ "hello" | string.slice1 1 3 }} {{ "hello" | string.slice1 1 length: 3 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] h e ell ell
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.split
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.split <text> <match>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The split function takes on a substring as a parameter. The substring is used as a delimiter to divide a string into an array. You can output different parts of an array using array functions.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] match : The string used to split the input text string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] An enumeration of the substrings
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ for word in "Hi, how are you today?" | string.split ' ' ~}} {{ word }} {{ end ~}}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Hi, how are you today?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.starts_with
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.starts_with <text> <value>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a boolean indicating whether the input string starts with the specified string value .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] value : The string to look for
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] if text starts with the specified string value
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "This is easy" | string.starts_with "This" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] true
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.strip
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.strip <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes any whitespace characters on the left and right side of the input string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string without any left and right whitespace characters
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ ' too many spaces ' | string.strip }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Highlight to see the empty spaces to the right of the string output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] too many spaces
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.strip_newlines
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.strip_newlines <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Removes any line breaks/newlines from a string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string without any breaks/newlines characters
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "This is a string.\r\n With \nanother \rstring" | string.strip_newlines }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] This is a string. With another string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_int
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_int <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a string to an integer
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A 32 bit integer or null if conversion failed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "123" | string.to_int + 1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 124
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_long
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_long <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a string to a long 64 bit integer
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A 64 bit integer or null if conversion failed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "123678912345678" | string.to_long + 1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 123678912345679
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_float
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_float <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a string to a float
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A 32 bit float or null if conversion failed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "123.4" | string.to_float + 1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 124.4
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_double
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.to_double <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a string to a double
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A 64 bit float or null if conversion failed
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "123.4" | string.to_double + 1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 124.4
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.truncate
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.truncate <text> <length> <ellipsis>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Truncates a string down to the number of characters passed as the first parameter. An ellipsis (...) is appended to the truncated string and is included in the character count
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] length : The maximum length of the output string, including the length of the ellipsis
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ellipsis : The ellipsis to append to the end of the truncated string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The truncated input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "The cat came back the very next day" | string.truncate 13 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The cat ca...
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.truncatewords
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.truncatewords <text> <count> <ellipsis>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Truncates a string down to the number of words passed as the first parameter. An ellipsis (...) is appended to the truncated string.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] count : The number of words to keep from the input text string before appending the ellipsis
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] ellipsis : The ellipsis to append to the end of the truncated string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The truncated input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "The cat came back the very next day" | string.truncatewords 4 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The cat came back...
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.upcase
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.upcase <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts the string to uppercase
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string upper case
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.upcase }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] TEST
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.md5
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.md5 <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Computes the md5 hash of the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The md5 hash of the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.md5 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 098f6bcd4621d373cade4e832627b4f6
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.sha1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.sha1 <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Computes the sha1 hash of the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The sha1 hash of the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.sha1 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] a94a8fe5ccb19ba61c4c0873d391e987982fbbd3
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.sha256
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.sha256 <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Computes the sha256 hash of the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The sha256 hash of the input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.sha256 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.hmac_sha1
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.hmac_sha1 <text> <secretKey>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a string into a SHA-1 hash using a hash message authentication code (HMAC). Pass the secret key for the message as a parameter to the function.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] secretKey : The secret key
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The SHA-1 hash of the input string using a hash message authentication code (HMAC)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.hmac_sha1 "secret" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 1aa349585ed7ecbd3b9c486a30067e395ca4b356
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.hmac_sha256
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.hmac_sha256 <text> <secretKey>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Converts a string into a SHA-256 hash using a hash message authentication code (HMAC). Pass the secret key for the message as a parameter to the function.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] secretKey : The secret key
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The SHA-256 hash of the input string using a hash message authentication code (HMAC)
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "test" | string.hmac_sha256 "secret" }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] 0329a06b62cd16b33eb6792be8c60b158d89a2ee3a876fce9a881ebb488c0914
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pad_left
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pad_left <text> <width>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Pads a string with leading spaces to a specified total length.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] width : The number of characters in the resulting string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string padded
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] hello{{ "world" | string.pad_left 10 }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] hello world
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pad_right
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.pad_right <text> <width>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Pads a string with trailing spaces to a specified total length.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The input string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] width : The number of characters in the resulting string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The input string padded
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "hello" | string.pad_right 10 }}world
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] hello world
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.base64_encode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.base64_encode <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Encodes a string to its Base64 representation. Its character encoded will be UTF-8.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to encode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The encoded string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "hello" | string.base64_encode }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] aGVsbG8=
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.base64_decode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.base64_decode <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Decodes a Base64-encoded string to a byte array. The encoding of the bytes is assumed to be UTF-8.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to decode
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The decoded string
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ "aGVsbG8=" | string.base64_decode }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] hello
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.index_of
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] string.index_of <text> <search> <startIndex>? <count>? <stringComparison>?
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Reports the zero-based index of the first occurrence of the specified string in this instance. The search starts at a specified character position and examines a specified number of character positions.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : The string to search
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] search : The string to find the index of.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] startIndex : If provided, the search starting position. If , search will start at the beginning of .
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] count : If provided, the number of character positions to examine. If , all character positions will be considered.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] stringComparison : If provided, the comparison rules for the search. If , Allowed values are one of the following: 'CurrentCulture', 'CurrentCultureIgnoreCase', 'InvariantCulture', 'InvariantCultureIgnoreCase', 'Ordinal', 'OrdinalIgnoreCase'
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] The zero-based index position of the parameter from the start of if is found, or -1 if it is not. If value is , the return value is (if is not provided, the return value would be zero).
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan functions
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan object represents a time interval.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Name Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .days Gets the number of days of this interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .hours Gets the number of hours of this interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .minutes Gets the number of minutes of this interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .seconds Gets the number of seconds of this interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .milliseconds Gets the number of milliseconds of this interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .total_days Gets the total number of days in fractional part
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .total_hours Gets the total number of hours in fractional part
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .total_minutes Gets the total number of minutes in fractional part
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .total_seconds Gets the total number of seconds in fractional part
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] .total_milliseconds Gets the total number of milliseconds in fractional part
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_days
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_hours
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_minutes
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_seconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_milliseconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.parse
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_days
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_days <days>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a timespan object that represents a days interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] days : The days.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ (timespan.from_days 5).days }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_hours
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_hours <hours>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a timespan object that represents a hours interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] hours : The hours.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ (timespan.from_hours 5).hours }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_minutes
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_minutes <minutes>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a timespan object that represents a minutes interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] minutes : The minutes.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ (timespan.from_minutes 5).minutes }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_seconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_seconds <seconds>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a timespan object that represents a seconds interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] seconds : The seconds.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ (timespan.from_seconds 5).seconds }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_milliseconds
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.from_milliseconds <millis>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns a timespan object that represents a milliseconds interval
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] millis : The milliseconds.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan object
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] input
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] {{ (timespan.from_milliseconds 5).milliseconds }}
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] output
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] :top:
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.parse
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] timespan.parse <text>
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Description
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Parses the specified input string into a timespan object.
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Arguments
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] text : A timespan text
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Returns
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] A timespan object parsed from timespan
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Examples
[ITPIE:OPS Documentation | Builtins | https://itpie-hostname/documentation/content/appendix/third-party/scriban/builtins.html] Note: This document was automatically generated from the sourcecode using Scriban.DocGen program
