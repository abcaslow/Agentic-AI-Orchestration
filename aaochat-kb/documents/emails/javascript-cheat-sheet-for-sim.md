Subject: Javascript cheat sheet for sim
From: Unitedwithcode <unitedwithcode@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Unitedwithcode <unitedwithcode@gmail.com> (Wed, 14 Oct 2026 13:51:02 -0400) ---
A JavaScript function is a reusable block of code designed to perform a
particular task, which executes whenever it is invoked or called. In
JavaScript, functions are considered first-class objects because they can
be assigned to variables, passed as arguments to other functions, and
returned from functions just like any other data type. [1
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions>
, 2 <https://www.youtube.com/watch?v=HFaxylC7bUc>, 3
<https://www.geeksforgeeks.org/javascript/difference-between-methods-and-functions-in-javascript/>
, 4 <https://web.dev/learn/javascript/functions>]

------------------------------

Core Structure of a Function

A standard function definition (or declaration) consists of the following
components: [1
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions>]

 1.

 The function keyword: Signals the creation of a function. [1
 <https://www.javascript.com/learn/functions>]
 2.

 The Name: A unique identifier used to call the function later (written
 in camelCase). [1 <https://www.youtube.com/watch?v=GyKxwS6dUXk&t=435>, 2
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions>
 ]
 3.

 Parameters: A list of placeholders enclosed in parentheses () that act
 as inputs. [1
 <https://www.geeksforgeeks.org/javascript/functions-in-javascript/>, 2
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions>
 ]
 4.

 The Body: A sequence of statements enclosed in curly braces {} that
 define what the function does. [1
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions>
 ]
 5.

 The return statement: Optional. Exits the function and outputs a
 specific value. If omitted, the function returns undefined by default. [1
 <https://rootstack.com/en/blog/how-do-javascript-functions-work>, 2
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions>
 , 3 <https://www.javascript.com/learn/functions>]

javascript

// Function Declaration

function greetUser(userName) {

 return `Hello, ${userName}!`;

}

// Function Invocation (Calling the function)

greetUser("Alice"); // Outputs: "Hello, Alice!"

The JavaScript const declaration creates a block-scoped local variable
whose value cannot be changed through reassignment. Introduced in ECMAScript
2015 (ES6), it establishes an immutable binding (or reference) to a value
rather than making the value itself immutable. [1
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>
, 2 <https://www.geeksforgeeks.org/javascript/javascript-const/>]

------------------------------

Core Characteristics

 -

 Mandatory Initialization: You must assign a value at the exact moment of
 declaration. Leaving it unassigned throws a SyntaxError. [1
 <https://www.w3schools.com/js/js_const.asp>, 2
 <https://mimo.org/glossary/javascript/const>, 3
 <https://www.javascripttutorial.net/javascript-const/>, 4
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>
 ]
 -

 No Reassignment: Attempting to assign a new value to the same variable
 name using an assignment operator (like =) will throw a TypeError. [1
 <https://mimo.org/glossary/javascript/const>, 2
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>
 ]
 -

 Block Scoping: The variable is strictly confined to the block { ... },
 function, or loop where it is defined. It does not bleed into outside
 scopes. [1
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>
 , 2 <https://mimo.org/glossary/javascript/const>]
 -

 No Redeclaration: You cannot redeclare a const variable within the same
 scope using const, let, or var. [1
 <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>
 , 2 <https://www.w3schools.com/js/js_const.asp>] ------------------------------

The "Constant" Misconception: Reassignment vs. Mutation

A critical distinction when using const is that it protects the variable
identifier reference, not the internal data structure. [1
<https://www.joshwcomeau.com/javascript/the-const-deception/>, 2
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>
]

Data Type

Reassignment (=)

Internal Mutation (Modifying contents)

Primitives (Numbers, Strings, Booleans)

❌ Forbidden (Throws error)

❌ N/A (Primitives are inherently immutable)

Objects & Arrays

❌ Forbidden (Throws error)

Allowed (Can change properties or push elements)

For example, a user consensus on Reddit
<https://www.reddit.com/r/learnprogramming/comments/sknavl/can_someone_help_me_understand_the_use_of_const/>
points out that const guarantees a variable won't point to something
entirely new, but as noted on MDN Web Docs
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>,
you are perfectly free to update an object's properties or push items into
an array. [1
<https://www.reddit.com/r/learnprogramming/comments/sknavl/can_someone_help_me_understand_the_use_of_const/>
, 2
<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const>
, 3 <https://mimo.org/glossary/javascript/const>]

If you would like to explore this further, I can provide code syntax
examples comparing const, let, and var, or show you how to completely
freeze an object so its properties cannot be changed. Which path should we
take? [1
<https://medium.com/@codingsam/what-really-is-a-constant-in-javascript-and-what-it-is-not-d3a8a9f655c2>
]

sim.ai Function Block

The Function block in Sim AI <https://www.sim.ai/> (an open-source AI
workflow and agent builder) is a deterministic step that executes custom
JavaScript, Python, or Shell code right inside your workflow. [1
<https://docs.sim.ai/workflows/blocks/function>, 2
<https://docs.sim.ai/workflows>]

What the JavaScript Function Block Does

 -

 Reshapes Data: Parse, filter, map, or transform JSON payloads and
 outputs coming from previous LLM or API blocks. [1
 <https://docs.sim.ai/workflows/blocks/function>]
 -

 Runs Calculations: Perform custom math, date formatting, string
 manipulation, or logic that standard model prompts or low-code blocks
 cannot handle reliably. [1
 <https://docs.sim.ai/workflows/blocks/function>]
 -

 Integrates Helpers: Access built-in platform utilities (such as reading
 uploaded files via sim.files helpers in plain JavaScript). [1
 <https://docs.sim.ai/workflows/blocks/function>]
 -

 Bridges Steps: Pass data seamlessly using angle-bracket syntax (e.g.,
 <api.data>) to reference upstream block outputs directly as code
 variables. [1 <https://docs.sim.ai/workflows/blocks/function>]

Example JavaScript Code Inside Sim

javascript

// Reference an upstream block output named 'api'

const data = <api.data>;

// Filter active items and extract their IDs

return data.items

 .filter((item) => item.active)

 .map((item) => item.id);

Use code with caution.

Execution Modes in Sim

 -

 Plain JavaScript (No Imports): Runs locally in an isolated in-process VM
 sandbox with zero extra configuration. [1
 <https://docs.sim.ai/platform/self-hosting>]
 -

 JavaScript with Imports / Python / Shell: Requires a configured remote
 sandbox provider (such as E2B or Daytona) and an active plan or self-hosted
 environment variable (SANDBOXES_ENABLED). [1
 <https://docs.sim.ai/platform/self-hosting>]

If you'd like, let me know:

 -

 What input data you are trying to process
 -

 What output format you need for the next block

I can write the exact JavaScript snippet for your Sim workflow.
