# ECMAScript 2015 (ES6)
---
## Introduction

ECMAScript 6, also known as ECMAScript 2015, is the latest version of the ECMAScript standard. ES6 is a significant update to the language, and the first update to the language since ES5 was standardized in 2009.

## JavaScript vs. ECMAScript
JavaScript was created in May 1995 by Brendan Eich while at Netscape, reportedly in only 10 days. It was originally named Mocha, a name chosen by Netscape founder Marc Andreessen, but was renamed four months later to LiveScript. At that time, Sun Microsystems owned the trademark for JavaScript. Netscape acquired a trademark license and renamed LiveScript to JavaScript in December 1995. It was somewhat of a marketing maneuver since Java was really popular at the time. The languages are not related at all.

Some time between 1996 and 1997, Netscape took JavaScript to the Ecma standards organization to carve out and maintain a specification for the language to enable other browser vendors to implement based on the work they had done. The Ecma Technical Committee 39 (better known as TC39) was created to continue to evolve the language, eventually releasing ECMA-262 Ed.1 in June 1997. ECMAScript is name of the official standard with JavaScript being the most well-known implementation of the standard. ActionScript (Macromedia) and JScript (Microsoft) are examples of other implementations.

Versions of JavaScript are defined by the specification that bears the official name of the language. For example, the first standard version of JavaScript was ECMAScript 1. It’s common practice now to abbreviate the standards specification to simply ES_X_, although the X will be changing in 2016 as TC39 shifts to a yearly release cadence. More on that towards the end of this post. All features in ECMAScript go through a formal proposal process. A proposal for a new feature, usually originating from the developer community, begins with a sketch or “strawman proposal” that provides an initial description of the proposed feature. If TC39 agrees that the feature is valuable, it will be promoted to official “Proposal” status. The deadline for ES6 proposals was way back in May 2011.

The next status is “In Implementation” where the feature is actually implemented in ideally 2 JavaScript engines. These implementations, as well as developer community feedback, help shape the proposal during its evolution. Finally if the proposal continues to prove to be valuable, TC39 will accept and it will be added to the next version of ECMAScript. It is now a “Standard.”

## ECMAScript 1, 2 & 3: The early days

ECMAScript 1, the first version of the JavaScript language standard, was released in June 1997. Exactly a year later, ECMAScript 2 was released, which contained only minor changes to keep in sync with a parallel ISO standard for JavaScript. 18 months later in December 1999, ECMAScript 3 was released, introducing a lot of the popular features of JavaScript that we now take for granted like regular expressions, try/catch exception handling, and formatting for numeric output.
## ECMAScript 4: The abandoned specification

Work began on ECMAScript 4 in early 2000 as an huge upgrade to ES3 and was even codenamed JavaScript 2. In 2003, the committee released an interim report that only contained some of the functionality earmarked for ES4. Microsoft’s JScript and Adobe’s ActionScript had implemented some of its features, but work stopped completely on the ES4 specification shortly after the interim report’s release.

Around this time, a new technique for creating dynamic client-side web applications using JavaScript emerged, which brought about a sort of JavaScript renaissance. JavaScript toolkit libraries like jQuery, Prototype, Dojo and Mootools were all released during this period of JavaScript rebirth. Jesse James Garrett coined this new approach Ajax in a white paper he wrote in February 2005. This white paper may very well be the reason why the TC39 elected to reconvene and resume work on ES4 in the Fall of 2005. It was to be based off of the now 7 year old ES3, the interim ES4 report, and learnings from ActionScript and JScript.

However, when the committee got together they were divided into 2 separate camps. In one corner was the “ECMAScript 4 Camp,” composed of Adobe, Mozilla, Opera & Google, who still wanted to work towards the massive upgrade. In the other corner was Microsoft & Yahoo, the “ECMAScript 3.1 Camp”, seeking a small subset of ES4, which would be more of an incremental upgrade of ES3 containing some minor features and bug fixes.

The rift ran pretty deep, but thankfully in July 2008 at a meeting in Oslo, Norway, a compromise was hashed out:

- Essentially what was ECMAScript 3.1 would become ECMAScript 5 — an incremental upgrade of ES3.
- TC39 would then develop a new major release that would be a scaled back version of the ambitious ES4, but bigger in scope than the incremental ES5. This major release was codenamed Harmony (due to the circumstances in which it was created) and would be for the most part what we now know as ECMAScript 6.
Some other features of the original ES4 plan would be dropped to be picked up in subsequent versions.
- The compromise did result in ECMAScript 4 being officially abandoned, but a renewed resolve was formed that any new ideas would be developed with the consensus of the entire TC39 in order to prevent the potential for future schisms.

## ECMAScript 5: The compromise specification

ECMAScript 5, the incremental upgrade to ES3, was released in December 2009, more than a decade after ES3. It is the version of JavaScript that is fully supported in all the browsers in use today except for Internet Explorer 8, of course.

It added several enhancements to the standard library such as:

- JSON parsing/serialization support
- Array prototype methods (like `map` and `forEach`)
- Methods for listing properties (like `Object.keys`).

There were also syntactic updates like:

- Allowances for dangling commas at the end of lists or object definitions
- Allowances for reserved words (like `new` or `for`) as object properties
Finally, it introduced strict mode, which made JavaScript a cleaner language by forbidding some features, performing additional runtime checks, and throwing more exceptions.

## ECMAScript 6: The new hotness

ECMAScript 6, which we will be learning about in great detail over a series of blog posts, was originally planned to be released in 2013, but wasn’t officially released until in June 2015. ECMAScript Harmony was the codename for the group of features following ES5, but it became clear that its goals were still too ambitious, so TC39 decided to break it up into two phases:

- The highest priority features would be in the next release of ECMAScript. It was codenamed ECMAScript.next in order to try to avoid the whole numbering fiasco with the lost ECMAScript 4.
- The remaining features would find their way into the following version.
As ECMAScript.next matured, the code name was dropped and it began going by ECMAScript 6, or simply, ES6. However, in late 2014, TC39 decided to rename ECMAScript 6 to ECMAScript 2015 in light of the new plan to release ECMAScript on a yearly cadence. By this time the standard was already well-established as ECMAScript 6, so most people still know it as ES6 and refer to it as such.

ES6 features are slowly rolling into the interpreters of our modern browsers and servers. The ES6 compatibility table tracks just how much of the standard each engine supports. As of writing, Microsoft’s new Edge browser is actually leading the pack with 67% of ES6 features supported. Firefox 11 (released in March 2012) was the first browser with “significant” support (more than 10%). Transpilers like Babel and Tracer let you compile a lot of ES6 down to valid ES5 for cross-browser compatibility. More on this in a future blog post.

