# Language

Source: ITPIE:OPS Documentation — Language
Source URL: https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Language
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This document describes the syntax of the scriban language in a templating context (within {{ and }} ).
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The language rules are the same in a pure scripting context.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] NOTE: This document does not describe the liquid language. Check the liquid website directly.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Table of Contents
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1. Blocks
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.1 Code block
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.2 Text block
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.3 Escape block
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.4 Whitespace control
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.5 Auto indentation
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 2 Comments
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3 Literals
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.1 Strings
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.2 Numbers
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.3 Boolean
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.4 null
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4 Variables
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4.1 The special variable this
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4.2 The special variable empty
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 5 Objects
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 5.1 The special property empty?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 6 Arrays
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 6.1 Array with properties
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 6.2 The special size property
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7 Functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.1 Simple functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.2 Anonymous functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.3 Parametric functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.4 Inline functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.5 Function Pointers
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8 Expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.1 Variable path expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.2 Assign expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.3 Nested expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.4 Arithmetic expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] On numbers
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] On strings
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.5 Conditional expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.6 Unary expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.7 Range expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.8 The null-coalescing operators ?? , ?!
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.9 Function call expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Named arguments
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9 Statements
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.1 Single expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.2 Compound Assignment
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.3 if <expression> , else , else if <expression>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Truthy and Falsy
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.4 case and when
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.5 Loops
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] for <variable> in <expression> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The offset parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The limit parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The reversed parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] while <expression> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] tablerow <variable> in <expression> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The cols parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Special loop variables
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] break and continue
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.6 capture <variable> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.7 readonly <variable>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.8 import <variable_path>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.9 with <variable> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.10 wrap <function> <arg1...argn> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.11 include <name> arg1?...argn?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.12 ret <expression>?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1. Blocks
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] There are 3 types of block of text in a template:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Code block : contains scriban template statements
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Text block : a plain block to output as is
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Escape block : a text block that can escape code blocks
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.1 Code block
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A text enclosed by {{ and }} is a scriban code block that will be evaluated by the scriban templating engine.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A scriban code block may contain:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] a single line expression statement : {{ name }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] or a multiline statements :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ if !name name = "default" end name }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] or statements separated by a semi-colon ; to allow compact forms in some use cases:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{if !name; name = "default"; end; name }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] In a code block, white space characters have no impact on parsing, with the exception of the end-of-line character following each statement. The only exception is when white space is used to distinguish between an array indexer and an array initializer.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Additionally, when a statement is an expression (but not an assignment expression), the result of the expression will be displayed in the template's output:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ x = 5 # This assignment will not output anything x # This expression will print 5 x + 1 # This expression will print 6 }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note that in the previous example, there is no EOL between 5 and 6 because we are inside a code block. You can still use a plain string with an EOL inside a code block "\n" or you could use mixed code and text blocks:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ x = 5 }} {{ x }} {{ x + 1 }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 5 6
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.2 Text block
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Otherwise, any text is treated as a text block and is outputted without modification.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Hello this is {{ name }}, welcome to scriban! ______________ _____________________ ^ text block ^ text block
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.3 Escape block
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Any code and text block can be escaped to produce a text block by enclosing it with {%{ and }%}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] For example the following escape:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input : {%{Hello this is {{ name }}}%} output : Hello this is {{ name }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] If you want to escape an escape block, you can increase the number of % in the starting and ending block:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input : {%%{This is an escaped block: }%} here}%%} output : This is an escaped block: }%} here
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This allow effectively to nest escape blocks and still be able to escape them.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This allows for effective nesting of escape blocks and the ability to escape them. For example, a starting escape block {%%%%{ will require an ending }%%%%}"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.4 Whitespace control
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] By default, any whitespace (including new lines) before or after a code/escape block are copied as-is to the output.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Scriban provides two modes for controlling whitespace:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The greedy mode using the character - (e.g {{- or -}} ), removes any whitespace, including newlines Examples with the variable name = "foo" :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Strip whitespace on the left:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a < {{- name}}> text
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a <foo> text
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Strip on the right:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a <{{ name -}} > text:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a <foo> text
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Strip on both left and right:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a < {{- name -}} > text:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a <foo> text
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The non greedy mode using the character ~
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Using a {{~ will remove any preceeding whitespace until it reaches a non whitespace character such as a newline or letter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Using a ~}} will remove any following whitespace including the first newline until it reaches a non whitespace character or a second newline
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This mode is very convenient when you want to use only a scriban statement on a line, but want that line to be completely removed from the output, but to keep spaces before and after this line intact.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] In the following example, we want to remove entirely the lines {{~ for product in products ~}} and {{~ end ~}} , but we want for example to keep the indentation of the opening <li> .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Using the greedy mode {{- or -}} would have removed all whitespace and lines and would have put the results on a single line.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <ul> {{~ for product in products ~}} <li>{{ product.name }}</li> {{~ end ~}} </ul>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <ul> <li>Orange</li> <li>Banana</li> <li>Apple</li> </ul>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Both mode ~ and '-' can also be used with escape blocks {%%{~ or ~}%%} or {%%{- or -}%%}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.5 Auto indentation
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] By default, when a code enter is without a left strip (e.g {{- or {{~ ) and is preceded by only whitespace on the same line, the content of the block will be indented accordingly to the number of whitespace before the code enter.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a_multi_line_value = "test1\ntest2\ntest3\n" ~}} {{ a_multi_line_value }}Hello
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Notice the 3 whitespace characters before the expression {{ a_multi_line_value }} .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] test1 test2 test3 Hello
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The output is auto-indented. This feature can be turned off on by setting TemplateContext.AutoIndent = false .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note that if the previous line contains a greedy right strip -}} , the indent will be skipped on the next code enter of the next line.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a_multi_line_value = "test1\ntest2\ntest3\n" -}} {{ a_multi_line_value }}Hello
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] test1 test2 test3 Hello
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 2 Comments
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Within a code block, scriban supports single line comments # and multi-line comments ## :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ name # this is a single line comment }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ ## This is a multi line comment ## }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] As you can notice, both single line and multi-line comments can be closed by the presence of a code block exit tag }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3 Literals
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.1 Strings
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Scriban supports two types of strings:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] regular strings enclosed by double quotes "..." or simple quotes '...' . Regular strings supports multiline and will interpret the following escape sequences:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \' single quote
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \" double quote
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \\ backslash
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \n new line
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \r carriage return
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \t tab
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \b backspace
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \f form feed
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \uxxxx where xxxx is a unicode hexa code number 0000 to ffff
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] \x00-\xFF a hexadecimal ranging from 0x00 to 0xFF
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] verbatim strings enclosed by backstick quotes `...` . They are, for example, useful to use with for regex patterns :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ "this is a text" | regex.split `\s+` }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] [this, is, a, text]
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Interpolated strings starting with a $ enclosed by double quotes $"..." or simple quotes $'...' .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ $"this is an interpolated string with an expression {1 + 2} and a substring {"Hello"}" }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] this is an interpolated string with an expression 3 and a substring Hello
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.2 Numbers
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A number in scriban {{ 100 }} is similar to a javascript number:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Integers: 100 , 1e3
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Hexadecimal integers: 0x1ef and unsigned 0x80000000u
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Floats: 100.0 , 1.0e3 , 1.0e-3
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 32-bit floats: 100.0f
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 64-bit floats: 100.0d
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 128-bit decimals: 100.0m
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.3 Boolean
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The boolean value {{ true }} or {{ false }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ true }} {{ false }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] true false
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3.4 null
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The null value {{ null }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] When resolving to a string output, the null value will output an empty string:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ null }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4 Variables
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Scriban supports the concept of global and local variables
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A global/property variable like {{ name }} is a liquid like handle, starting by a letter or underscore _ and following by a letter A-Z a-z , a digit 0-9 , an underscore _
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following text are valid variable names:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] var
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] var9
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] _var
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] NOTE: In liquid, the character - is allowed in a variable name, but when translating it to a scriban, you will have to enclose it into a quoted string
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A local variable like {{ $name }} is an identifier starting with $ . A local variable is only accessible within the same include page or function body.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The special local variable $ alone is an array containing the arguments passed to the current function or include page.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The special local variables $0 $1 ... $n is a shorthand of $[0] , $[1] ... $[n] . e.g Using $0 returns the first argument of the current function or including page.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4.1 The special variable this
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The this variable gives you access to the current object bound where you have access to all local variables for the current scope.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Thus the following variable access are equivalent:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a = 5 a # output 5 this.a = 6 a # output 6 this["a"] = 7 a # output 7 }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 567
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] In the case of the with statement, the this operator refers to the object passed to with :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a = {x: 1, y: 2} with a b = this end b.x }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4.2 The special variable empty
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The empty variable represents an empty object and is primarily used for compatibility with Liquid templates. It provides a way to compare an object with the empty variable to determine if it is empty or not:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a = {} b = [1, 2]~}} {{a == empty}} {{b == empty}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] true false
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 5 Objects
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Scriban supports javascript like objects {...}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An object can be initialized empty:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject = {} }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An object can be initialized with some members:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject = { member1: "yes", member2: "no" } }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] or use a json syntax:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject = { "member1": "yes", "member2": "no" } }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An object can be initialized with some members over multiple lines:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject = { member1: "yes", member2: "no" } }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Members of an object can be accessed using dot notation or square bracket notation:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject.member1 }} also equivalent to {{ myobject["member1"] }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] You can access optional members in chain via the optional member operator ?. (instead of the regular member operator: . ) ( New in 3.0 )
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject.member1?.submember1?.submember2 ?? "nothing" }} will return "nothing" as member1 doesn't contain a submember1 / submember2 .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] If the object is a "pure" scriban objects (created with a {...} or instantiated by the runtime as a ScriptObject ), you can also add members to it with a simple assignment:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject = {} myobject.member3 = "may be" myobject.member3 }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] may be
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] NOTICE
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] By default, Properties and methods of .NET objects are automatically exposed with lowercase and _ names. It means that a property like MyMethodIsNice will be exposed as my_method_is_nice . This is the default convention, originally to match the behavior of liquid templates. If you want to change this behavior, you need to use a MemberRenamer delegate
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 5.1 The special property empty?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Any object can respond the the property .empty? to check if it is empty or not:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a = {} b = [1, 2]~}} {{a.empty?}} {{b.empty?}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] true false
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 6 Arrays
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An array can be initialized empty:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myarray = [] }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An array can be initialized with some items:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myarray = [1, 2, 3, 4] }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An array can be initialized with some items over multiple lines:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myarray = [ 1, 2, 3, 4, ] }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Items of an array can be zero-based indexed:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myarray[0] }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] If the array is a "pure" scriban array (created with a [...] or instantiated by the runtime as a ScriptArray ), you can also add items to it with a simple assignment that will expand automatically the array depending on the index:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myarray = [] myarray[0] = 1 myarray[1] = 2 myarray[2] = 3 myarray[3] = 4 }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] You can also manipulate arrays with the array builtin object .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Important notice
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] While whitespace characters are mostly not relevant while parsing in scriban, there is a case where a whitespace helps to disambiguate between an array indexer and an array initializer .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] For instance, if a whitespace is found before a [ and the previous expression was a variable path expressions (see later), the following expression [...] will be considered as an array initializer instead of an array indexer:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myfunction [1] # There is a whitespace after myfunction. # It will result in a call to myfunction passing an array as an argument myvariable[1] # Without a whitespace, this is accessing # an element in the array provided by myvariable }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 6.1 Array with properties
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An array can also contains attached properties:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a = [5, 6, 7] a.x = "yes" a.x + a[0] }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] yes5
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 6.2 The special size property
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Arrays have a size property that can be used to query the number of elements in the array:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ a = [1, 2, 3] a.size }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7 Functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Scriban allows for the definition of four different types of functions:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Simple functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Anonymous functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Parametric functions ( New in 3.0 )
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Inline functions ( New in 3.0 )
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.1 Simple functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following declares a function sub that takes two arguments, a and b , and subtracts the value of b from a :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{func sub ret $0 - $1 end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] All argument are passed to the special variable $ that will contain the list of direct arguments and named arguments:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] $0 or $[0] will access the first argument
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] $1 or $[1] will access the second argument
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] $[-1] will access the last argument
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] $.named will access the named argument named
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This function can then be used:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{sub 5 1}} {{5 | sub 1}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4 4
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] As you can notice from the example above, when using the pipe, the result of the pipe is pushed as the first argument of the pipe receiver.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note that a function can have mixed text statements as well:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{func inc}} This is a text with the following argument {{ $0 + 1 }} {{end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] NOTE: Setting a non-local variable (e.g a = 10 ) in a simple function will be set at the global level and not at the function level.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Parametric functions are solving this behavior by introducing a new variable scope inside the function that includes parameters.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.2 Anonymous functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Anonymous functions are like simple functions but can be used in expressions (e.g as the last argument of function call)
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ sub = do; ret $0 - $1; end; 1 | sub 3 }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] They are very convenient to build custom block functions:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ func launch; ret $0 1 2; end launch do ret $0 + $1 end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.3 Parametric functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] They are similar to simple functions but they are declared with parenthesis, while also supporting declaration of different kind of parameters (normal, optional, variable).
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Another difference with simple functions is that they require function calls and arguments to match the expected function parameters.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A function with normal parameters:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{func sub(x,y) ret x - y end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{sub 5 1}} {{5 | sub 1}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4 4
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A function with normal parameters and optional parameters with default values:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{func sub_opt(x, y, z = 1, w = 2) ret x - y - z - w end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{sub_opt 5 1}} {{5 | sub_opt 1}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1 1
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Here we override the value of z and set it to 0 instead of default 1 :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{sub_opt 5 1 0 }} {{5 | sub_opt 1 0}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 2 2
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A function with normal parameters and optional parameters with default values:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{func sub_variable(x, y...) ret x - (y[0] ?? 0) - (y[1] ?? 0) end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{sub_variable 5 1 -1} {{5 | sub_variable 1 -1}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 5 5
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] NOTE: The special variable $ is still accessible in parametric functions and represent the direct list of arguments. In the example above, $ = [5, [1, -1]]
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.4 Inline functions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] For simple functions, it is convenient to define simple functions like mathematical functions:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ sub(x,y) = x - y }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Inline functions are similar to parametric functions but they only support normal parameters. They don't support optional or variable parameters.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 7.5 Function Pointers
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Because functions are object, they can be stored into a property of an object by using the alias @ operator:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject.myinc = @inc # Use the @ alias operator to allow to # use a function without evaluating it x = 1 | myobject.myinc # x = x + 1 }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The function aliasing operator @ allows to pass a function as a parameter to another function, enabling powerful function compositions.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8 Expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Scriban supports conventional unary and binary expressions.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.1 Variable path expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A variable path expression contains the path to a variable:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A simple variable access: {{ name }} e.g resolve to the top level variable name
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An array access: {{ myarray[1] }} e.g resolve to the top level variable myarray and an indexer to the array
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A member access: {{ myobject.member1.myarray[2] }} e.g resolve to the top level variable myobject , then the property member1 this object, the property myarray and an indexer to the array returned by myarray
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note that a variable path can either point to a simple variable or can result into calling a parameter less function.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.2 Assign expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A value can be assigned to a top level variable or to the member of an object/array:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ name = "foo" }} e.g Assign the string "foo" the variable name
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject.member1.myarray[0] = "foo" }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An assign expression must be a top level expression statement and cannot be used within a sub-expression.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.3 Nested expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An expression enclosed by ( and )
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ name = ('foo' + 'bar') }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.4 Arithmetic expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] On numbers
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following binary operators are supported for numbers :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Operator Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> + <right> add left to right number
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> - <right> subtract right number from left
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> * <right> multiply left by right number
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> / <right> divide left by right number
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> // <right> divide left by right number and round to an integer
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> % <right> calculates the modulus of left by right
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] If left or right is a float and the other is an integer, the result of the operation will be a float.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] On strings
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following binary operators are supported for strings :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Operator Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 'left' + <right> concatenates left to right string: "ab" + "c" -> "abc"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 'left' * <right> concatenates the left string right times: 'a' * 5 -> aaaaa . left and right and be swapped as long as there is one string and one number.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] As long as there is a string in a binary operation, the other part will be automatically converted to a string.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following literals are converted to plain strings:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] null -> "" . e.g: "aaaa" + null -> "aaaa"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 0 -> "0"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1.0 -> "1.0"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] true -> "true"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] false -> "false"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.5 Conditional expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A boolean expression produces a boolean by comparing a left and right value.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Operator Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> == <right> Is left equal to right?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> != <right> Is left not equal to right?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> > <right> Is left greater than right?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> >= <right> Is left greater or equal to right?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> < <right> Is left less than right?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> <= <right> Is left less or equal to right?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] They work with both numbers , strings and datetimes.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] You can combine conditional expressions with && (and operator) and || (or operator). Unlike in javascript it always returns boolean and never <left> or <right> .
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Operator Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> && <right> Is left true and right true?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> \|\| <right> Is left true or right true?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The conditional expression cond ? left : right allow to return left if cond is true otherwise right . ( New in 3.0 )
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.6 Unary expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Operator Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] ! <expression> Boolean negate an expression. e.g if !page
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] + <expression> Arithmetic positive an expression. e.g +1.5
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] - <expression> Arithmetic negate an expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] ^ <expression> Expand an array passed to arguments of a function call (see function call)
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] @ <expression> Alias the result of an expression that would be evaluated if it was a function call
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] ++ <variable> Increments the variable. Expression is evaluated to the value after it is incremented.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] -- <variable> Decrements the variable. Expression is evaluated to the value after it is decremented.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <variable> ++ Increments the variable. Expression is evaluated to the value before it is incremented.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <variable> -- Decrements the variable. Expression is evaluated to the value before it is decremented.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note: For the increment an decrement operators, the operand must be a variable, property or indexer
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.7 Range expressions
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] They are special binary expressions that provides an iterator (used usually with the for statement)
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The evaluated left and right expressions must resolve to an integer at runtime.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Operator Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] left..right Returns an iterator between left and right with a step of 1, including right . e.g: 1..5 iterates from 1 to 5
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] left..<right Returns an iterator between left and right with a step of 1, excluding right . e.g: 1..<5 iterates from 1 to 4
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.8 The null-coalescing operators ?? , ?!
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The operator left ?? right can be used to return the right value if left is null.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The operator left ?! right can be used to return the right value if left is not null.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 8.9 Function call expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A function can be called by passing parameters separated by a whitespace:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myfunction arg1 "arg2" (1+5) }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The pipe operator | can also be used to pipe the result of an expression to a function:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ date.parse '2016/01/05' | date.to_string '%g' }} will output 06 Jan 2016
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Notice that when a function receives the result of a pipe call (e.g date.to_string in the example above), it is passed as the first argument of the call . This is valid for both .NET custom functions as well as for Scriban integrated functions.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Pipes are greedy with respect to whitespace. This allow them to be chained across multiple lines:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{- "text" | string.append "END" | string.prepend "START" -}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] will output STARTtextEND
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Named arguments
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] When passing multiple arguments to an existing .NET function, you may want to use named arguments.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Suppose you have declared a .NET function like this:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] public static string MyProcessor(string left, string right, int count, string options = null) { // ... }
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] You can call this function from scriban with the following syntax:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ my_processor "Hello" "World" count: 15 options: "optimized" }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] with a pipe we could rewrite this to:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ "Hello" | my_processor "World" count: 15 options: "optimized" }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note that once arguments are named, the following arguments must be all named.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] In a custom function declared with func named arguments are accessible through the variable arguments variable $ , but as properties (and not as part of the default array arguments):
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ func my_processor "Argument count:" + $.count "Argument options:" + $["options"] for $x in $ "arg[" + $x + "]: " + $x end end my_processor "Hello" "World" count: 15 options: "optimized" }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Argument count: 15 Argument options: optimized arg[0]: Hello arg[1]: World
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9 Statements
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Each statement must be terminated by a code block }} or an EOL within a code block, or a semicolon to separate multiple statements on a single line within a code block.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.1 Single expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An expression statement:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ value + 1 }} e.g Evaluates value + 1 and output the result
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ value + 1 # This is a single line expression statement followed by this comment }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.2 Compound Assignment
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following compound assignment operators are supported for numbers :
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Operator Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> += <right> add left to right number, and assigns the result to left
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> -= <right> subtract right number from left, and assigns the result to left
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> *= <right> multiply left by right number, and assigns the result to left
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> /= <right> divide left by right number, and assigns the result to left
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> //= <right> divide left by right number and round to an integer, and assigns the result to left
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <left> %= <right> calculates the modulus of left by right, and assigns the result to left
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] If left or right is a float and the other is an integer, the result of the operation will be a float.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note: The left-hand side of the assignment statement must be a variable, property or indexer
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.3 if <expression> , else , else if <expression>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The general syntax is:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ if <expression> ... else if <expression> ... else ... end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An if statement must be closed by an end or followed by a else or else if statement. An else or else if statement must be followed by a else , else if or closed by an end statement.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] An expression evaluated for a if or else if will be converted to a boolean.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Truthy and Falsy
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] By default, only the null and boolean false are considered as false when evaluated as booleans.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following values are used for converting literals to boolean:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 0 -> true
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1 -> true or any non zero value
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] null -> false
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] false -> false
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] non_null_object -> true
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] "" -> true An empty string returns true
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] "foo" -> true
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Example testing a page object:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ if page }}Page is not null{{ else }}Page is null!{{ end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.4 case and when
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is the equivalent of switch statement in C#, a selection statement that chooses a single switch section to execute from a list of candidates based on a value matching.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] case <expression> opens a switch with an expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] when <match> allows to match with the specified expression and the case expression
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] when can also be used with multiple values separated by , or ||
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] A final else can be used to as a default handler in case nothing matched.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ x = 5 case x when 1, 2, 3 "Value is 1 or 2 or 3" when 5 "Value is 5" else "Value is " + x end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Value is 5
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.5 Loops
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] for <variable> in <expression> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for <variable> in <expression>}} ... {{end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The expression can be an array or a range iterator:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Loop on an array: {{ for page in pages }}This is the page {{ page.title }}{{ end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Loop on a range: {{ for x in 1..n }}This is the loop step [{{x}}]{{ end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The for loop (along with the tablerow statement below) supports additional parameters, offset , limit and reversed that can also be used togethers:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The offset parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Allows to start the iteration of the loop at the specified zero-based index:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{~ for $i in (4..9) offset:2 ~}} {{ $i }} {{~ end ~}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 6 7 8 9
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The limit parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Limits the iteration of the loop to a specified count:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{~ for $i in (4..9) limit:2 ~}} {{ $i }} {{~ end ~}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 4 5
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The reversed parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Reverses the iteration of the elements:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{~ for $i in (1..3) reversed ~}} {{ $i }} {{~ end ~}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 3 2 1
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] while <expression> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{while <expression>}} ... {{end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Like the if statement, the expression is evaluated to a boolean.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] tablerow <variable> in <expression> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This function generates HTML rows compatible with an HTML table. Must be wrapped in an opening <table> and closing </table> HTML tags.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This statement is mainly for compatibility reason with the liquid tablerow tag. It uses similar syntax to a for statement (supporting the same parameters).
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{tablerow <variable> in <expression>}} ... {{end}}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <table> {{~ tablerow $p in products | array.sort "title" -}} {{ $p.title -}} {{ end ~}} </table>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <table> <tr class="row1"><td class="col1">Apple</td></tr> <tr class="row2"><td class="col1">Banana</td></tr> <tr class="row3"><td class="col1">Computer</td></tr> <tr class="row4"><td class="col1">Mobile Phone</td></tr> <tr class="row5"><td class="col1">Orange</td></tr> <tr class="row6"><td class="col1">Sofa</td></tr> <tr class="row7"><td class="col1">Table</td></tr> </table>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The cols parameter
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Defines the number of columns to output:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] input
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <table> {{~ tablerow $p in (products | array.sort "title") limit: 4 cols: 2 -}} {{ $p.title -}} {{ end ~}} </table>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] output
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] <table> <tr class="row1"><td class="col1">Apple</td><td class="col2">Banana</td></tr> <tr class="row2"><td class="col1">Computer</td><td class="col2">Mobile Phone</td></tr> </table>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Special loop variables
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The following variables are accessible within a for block:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Name Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for.index}} The current index of the for loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for.rindex}} The current index of the for loop starting from the end of the list
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for.first}} A boolean indicating whether this is the first step in the loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for.last}} A boolean indicating whether this is the last step in the loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for.even}} A boolean indicating whether this is an even row in the loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for.odd}} A boolean indicating whether this is an odd row in the loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{for.changed}} A boolean indicating whether a current value of this iteration changed from previous step
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Within a while statement, the following variables can be used:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Name Description
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{while.index}} The current index of the while loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{while.first}} A boolean indicating whether this is the first step in the loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{while.even}} A boolean indicating whether this is an even row in the loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{while.odd}} A boolean indicating whether this is an odd row in the loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] break and continue
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The break statement allows to early exit a loop
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ for i in 1..5 if i > 2 break end end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The continue statement allows to skip the rest of a loop and continue on the next step
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ for i in 1..5 if i == 2 continue end }} [{{i}}]] step {{ end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Will output:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] [1] step [3] step [4] step [5] step
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.6 capture <variable> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The capture <variable> ... end statement allows to capture the template output to a variable:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] For example the following code:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ capture myvariable }} This is the result of a capture {{ date.now }} {{ end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] will set myvariable = "This is the result of a capture 06 Jan 2016\n"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.7 readonly <variable>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The readonly statement prevents a variable for subsequent assignments:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ x = 1 }} {{ readonly x }} {{ x = 2 }} <- this will result in a runtime error
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.8 import <variable_path>
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The import <variable_path> statement allows to import the members of an object as variables of the current bound:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ myobject = { member1: "yes" } import myobject member1 # will print the "yes" string to the output }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note that readonly variables won't be override.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.9 with <variable> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The with <variable> ... end statement will open a new object context with the passed variable, all assignment will result in setting the members of the passed object.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] myobject = {} with myobject member1 = "yes" end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.10 wrap <function> <arg1...argn> ... end
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Pass a block of statements to a function that will be able to evaluate it using the special variable $$
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ func wrapped for $i in 1..<$0 $$ # This special variable evaluates the block pass # to the wrap statement end end wrap wrapped 5 $i + " -> This is inside the wrap!\r\n" end }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] will output:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 1 -> This is inside the wrap! 2 -> This is inside the wrap! 3 -> This is inside the wrap! 4 -> This is inside the wrap!
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] Note that variables declared outside the with block are accessible within.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.11 include <name> arg1?...argn?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] include is not a statement but rather a function that allows you to parse and render a specified template. To use this function, a delegate to a template loader must be setup on the TemplateOptions.TemplateLoader property passed to the Template.Parse method.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] include 'myinclude.html' x = include 'myinclude.html' x + " modified"
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] assuming that myinclude.html is
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] {{ y = y + 1 ~}} This is a string with the value {{ y }}
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] will output:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a string with the value 1 This is a string with the value 2 modified
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] 9.12 ret <expression>?
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] The return statement is used to early exit from a top-level/include page or a function.
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a text {{~ ret ~}} This text will not appear
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] will output:
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] This is a text
[ITPIE:OPS Documentation | Language | https://itpie-hostname/documentation/content/appendix/third-party/scriban/language.html] :top: