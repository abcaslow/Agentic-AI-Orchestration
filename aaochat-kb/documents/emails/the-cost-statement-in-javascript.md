Subject: The cost statement in javascript
From: Bruce Caslow <abcaslow@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Bruce Caslow <abcaslow@gmail.com> (Wed, 14 Oct 2026 05:02:44 -0400) ---
The *const statement in JavaScript is incredibly important* because it
serves as the foundation for writing predictable, readable, and modern
code. Introduced in ES6 (2015), it is now widely considered the *default
choice for variable declaration* in the developer community, outcompeting
let and rendering var virtually obsolete for standard use cases.
Here is a breakdown of why const is so critical, its core behaviors, and
the trade-offs you need to know.
------------------------------
Why const is Crucial

 - *Immutability of the Binding:* When you declare a variable with const,
 the reference to that value cannot be changed. If you try to reassign it,
 JavaScript will throw a TypeError. This prevents accidental bugs where
 variables are overwritten by mistake.
 - *Signal Intent (Readability):* Using const tells other developers (and
 your future self) that this value is meant to stay fixed throughout its
 lifecycle. It lowers the cognitive load required to read the code because
 you don't have to scan the rest of the file to see if the variable changes.
 - *Block Scoping:* Like let, const is block-scoped. This means it only
 exists within the nearest pair of curly braces {} (like in an if statement
 or a for loop), preventing variables from leaking into places they
 shouldn't.

------------------------------
The Big Catch: Objects and Arrays
A common point of confusion is that *const does not make values completely
immutable*. It only prevents *reassignment* of the variable itself.

 - *Primitives (Strings, Numbers, Booleans):* Completely protected. You
 cannot change their value.
 - *Objects and Arrays:* The *reference* is protected, but the *contents* can
 still be modified.

Action Allowed with const? Example
*Reassigning the variable* ❌ *No* const x = 5; x = 6; *(Throws Error)*
*Modifying an object property* *Yes* const user = { age: 20 }; user.age =
21; *(Allowed)*
*Pushing to an array* *Yes* const list =; list.push(3); *(Allowed)*
*Tip: If you want to make an object truly unchangeable, you have to
use Object.freeze(obj) alongside const.*
------------------------------
Best Practices

 1.
 - *Default to const:* Start every single variable declaration with
 const.
 - *Upgrade to let only when necessary:* If you realize later in your
 code that the variable *must* be reassigned (like a counter in a
 loop, or a toggled boolean), change it to let.
 - *Never use var:* Modern JavaScript standards discourage var entirely
 due to its confusing scoping rules (hoisting).

------------------------------
If you'd like, we can look at some code examples. Let me know:

 - Do you want to see *how block-scoping works* compared to old
 JavaScript?
 - Would you like to see how to *safely lock down objects* using
 Object.freeze()?
