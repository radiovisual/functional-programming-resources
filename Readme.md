##Functional Programming Resources

An archive of the best resources surrounding the functional programming paradigm.

> Object Orientation makes code understandable by encapsulating moving parts. Functional programming makes code understandable by minimizing moving parts. ~ Michael Feathers

Functional programming is making a strong comeback, and with it: a massive wave of internet buzz. Someone needs to sort the good from the bad, and that is what I will attempt to do here.
My focus is on the functional paradigm in the context of Javascript, but discussion and highlight of other Functional languages are welcome for the purpose of evaluation, comparison and education.

**Note:** This is very much a work in progress!

###Keywords

- **Higher-Order Functions** A fancy term for a function that accepts another function as an argument. *[source](http://www.quora.com/What-is-a-simple-explanation-of-higher-order-functions-and-callbacks-in-JavaScript)*
- **Currying** Currying is the process of transforming a function that takes multiple arguments into a function that takes just a single argument and returns another function if any arguments are still needed. *[source](http://tech.pro/tutorial/2011/functional-javascript-part-4-function-currying)*
- **Pure Functions** A pure function is a function that does not introduce any "side effects" by affecting state anywhere in your application. Pure functions return a value, and that is all they do. This keeps your functions clean, predictable, and highly-testable.
- **Functors** A functor is a container that you can map over; apply a function to its contents & return a new container with results. e.g. JS Arrays.
- **Monad** In functional programming, a monad is a structure that represents computations defined as sequences of steps: a type with a monad structure defines what it means to chain operations, or nest functions of that type together. This allows the programmer to build pipelines that process data in steps, in which each action is decorated with additional processing rules provided by the monad. *[source](http://en.wikipedia.org/wiki/Monad_%28functional_programming%29)*
- **Immutable** Immutable values are values that never change once instantiated. All variables (symbols) are immutable in functional languages.
- **Tail Call** A tail call happens when a function `F` makes a function call as its final action. At that point `F` will do absolutely no more work: it passes the ball to whatever function is being called and vanishes from the game. *[source](http://duartes.org/gustavo/blog/post/tail-calls-optimization-es6/)*

###Articles

- [Functional Programming for the Rest of Us](http://www.defmacro.org/ramblings/fp.html). This article has a really great way of explaining some of the heavier aspects of FP. It breaks out of the typically-academic approach; speaking directly to developers, and not an assembly of mathematicians.
- [Don't Be Scared of Functional Programming](http://www.smashingmagazine.com/2014/07/02/dont-be-scared-of-functional-programming/) via Smashing Magazine.
- [Why Curry Helps](http://hughfdjackson.com/javascript/why-curry-helps/) A great article on the beauties of currying.
- [The Two Pillars of JavaScript — Pt 2: Functional Programming](https://medium.com/javascript-scene/the-two-pillars-of-javascript-pt-2-functional-programming-a63aa53a41a4) Nice article by Eric Elliot on the topic of FP.
- [Functional Programming in Javascript](http://jhusain.github.io/learnrx/) Cool interactive lessons on FP in JS.
- [Promises + FP = Beautiful Streams ](http://tech.pro/blog/6888/promises--fp--beautiful-streams)
- [Bringing functional to the frontend: Clojure + ClojureScript for the web](http://blog.getprismatic.com/bringing-functional-to-the-frontend-clojure-clojurescript-for-the-web/)
- [Om sweet Om: (high-)functional frontend engineering with ClojureScript and React](http://blog.getprismatic.com/om-sweet-om-high-functional-frontend-engineering-with-clojurescript-and-react/)
- [Functional programming on frontend with React & ClojureScript](http://blog.scalac.io/2015/04/02/clojurescript-reactjs-reagent.html)

###Videos & Presentations

- [Simple Made Easy](http://www.infoq.com/presentations/Simple-Made-Easy) by Rich Hickney (author of Clojure)
- [React.js Conf 2015 - Immutable Data and React](https://www.youtube.com/watch?v=I7IdS-PbEgI) Not 100% about FP, but has some great tips on immutable data with the react.js library.
- [Functional Programming with Generators](https://www.youtube.com/watch?v=B2ASp0jb6FY)
- [An Introduction to Functional Reactive Programming](https://www.youtube.com/watch?v=ZOCCzDNsAtI)
- [Immutability: Putting The Dream Machine To Work](https://www.youtube.com/watch?v=SiFwRtCnxv4) by [David Nolen](https://twitter.com/swannodette)
- [Functional Programming with Generators](https://www.youtube.com/watch?v=B2ASp0jb6FY)
- [What if the user were a function?](https://www.youtube.com/watch?v=1zj7M1LnJV4) Great talk by [@andrestaltz](https://twitter.com/andrestaltz). Explores reactive / functional programming and more.

### Video Series: Functional Programming in Javascript

 Created by Mattias P Johansson [twitter](https://twitter.com/mpjme) | [youtube](https://www.youtube.com/channel/UCO1cgjhGzsSYb1rsB4bFe4Q)

- [Part 1: Higher-order functions](https://www.youtube.com/watch?v=BMUiFMZr7vk)
- [Part 2: Map](https://www.youtube.com/watch?v=bCqtb-Z5YGQ)
- [Part 3: Reduce Basics](https://www.youtube.com/watch?v=Wl98eZpkp-c)
- [Part 4: Reduce Advanced](https://www.youtube.com/watch?v=1DMolJ2FrNY)
- [Part 5: Closures](https://www.youtube.com/watch?v=CQqwU2Ixu-U)
- [Part 6: Currying](https://www.youtube.com/watch?v=iZLP4qOwY8I)
- [Part 7: Recursion](https://www.youtube.com/watch?v=k7-N8R0-KY4)
- [Part 8: Promises](https://www.youtube.com/watch?v=2d7s3spWAzo)

###Courses (free and paid)

- [Javascript: From Fundamentals to Functional JS](https://frontendmasters.com/courses/js-fundamentals-to-functional/) (Frontend Masters)
- [Hardcore Functional Programming in JavaScript](https://frontendmasters.com/courses/functional-javascript/) (Frontend Masters)
- [Introduction to Functional Programming](https://www.edx.org/course/introduction-functional-programming-delftx-fp101x#.VQaxMmTkcme) (edX)

###Benefits of Functional Programming

- **Unit Testing** No function can ever cause side-effects, there is no need to care about external state, or calling functions in any particular order, all you need to do is pass arguments to your functions that represent your edge cases, this makes unit testing *an absolute dream*, and your applications can ship with confidence!
- **Debugging** Debugging a functional program is a breeze. If a function doesn't behave appropriately, just take a peek at your stack, and all the functions and variables that lead you to this point are staring right at you. No need to examine any external state, or investigate who/what/where could have interfered, it's all right in front of you.
- **Concurrency** The functional programming paradigms offers concurrency as a bonus right out of the box. Nothing in a functional program is ever modified twice by the same thread, let alone by two different threads. There is never any need to use locks, or worry about race conditions. Add as many threads to your app as you want, and your program will keep humming away. Beautiful.
- **Hot Code Deployment** Ever wish you could update/patch your live application without having to shut the system down first? With FP, it's not a problem!
- **Machine-Assisted Proofs & Optimizations** Because functional languages share a common root in mathematics, tooling for optimizations, testing, evaluation, etc can be built to further demonstrate the validity of your application. See "[Machine Assisted Proofs and Optimizations](http://www.defmacro.org/ramblings/fp.html)" for more information.
- **Highly-Readable Code** FP is an extremely expressive design paradigm, and this expressiveness tends to lend itself to beautifully-crafted programs that are clear and concise.
- **Excellent Code Reuse** The FP paradigm supports modular, reusable code straight out of the box. This is because functions compose themselves of existing functions, so you get to decide how these functions are combined to perform your application logic.
- **Highly-Maintainable Code** FP programs are incredibly easy to read, due to the declarative (and modular) nature of functional programming. Additionally: Functional programs also tend to be shorter than their imperative counterparts, and a smaller code base is easier to maintain than a large one.
- **Static Types** In FP, all 'variables' (immutable symbols) have a type (either declared, or inferred at compile-time). The compiler can then analyse your code and help you avoid a wide range of common problems that plague developers in non statically-typed languages. Note: Javascript is not a statically-typed language, see the "Gotchas" section.

###The "Gotchas" of Javascript

Certain aspects of the javascript language make it tricky to harness the full power of a fully-functional language, namely:

- **Javascript is not a statically-typed language.** Variables in javascript are dynamically-typed, which means that they can change their type at anytime. This is counter to the functional methodology where all symbols are immutable and have an explicit type.
- **Variables are only immutable in ES6.** All ECMAScript specifications lower than 6 ( >= ES5 ) do not support immutable variables. Note that the `const` keyword is available in ES6, where variables declared like `const foo = 123;` are immutable, but objects declared with `const` behave differently (see the next gotcha).
- **In ES6, objects declared with `const` are mutable**. The idea here is that the *pointer reference to the object is immutable* when your object is declared with `const`, but the object itself is mutable.

###Libraries & Frameworks

- [Ramda](http://ramdajs.com/) A utility library with a focus on flexible functional composition enabled by automatic currying and reversed argument order. Avoids mutating data.
  - [Practical Functional Javascript with Ramda](http://developer.telerik.com/featured/practical-functional-javascript-ramda/)
  - [The Philosophy of Ramda](http://fr.umio.us/the-philosophy-of-ramda/)
- [functionaljs](http://functionaljs.com/) A functional JavaScript library. It facilitates currying and point-free / tacit programming and this methodology has been adhered to from the ground up.
- [lodash](http://lodash.com) - A utility library delivering consistency, customization, performance, & extras. A better and faster Underscore.js.
- [Mout](http://moutjs.com) - Utility library with the biggest difference between other existing solutions is that you can choose to load only the modules/functions that you need, no extra overhead.
- [mori](http://swannodette.github.io/mori/) - A library for using ClojureScript's persistent data structures and supporting API from the comfort of vanilla JavaScript.
- [Folktale](http://folktale.github.io) - A suite of libraries for generic functional programming in JavaScript that allows you to write elegant, modular applications with fewer bugs, and more reuse.
- [immutable](https://github.com/facebook/immutable-js) - Immutable data collections.
- [underscore-contrib](http://documentcloud.github.io/underscore-contrib/) - The brass buckles on Underscore's utility belt.
- [Bacon.js](http://baconjs.github.io) - Functional reactive programming.
- [RxJS](http://reactive-extensions.github.io/RxJS/) - Functional reactive library for transforming, composing, and querying various kinds of data.
- [Lazy.js](https://github.com/dtao/lazy.js/) - Utility library similar to lodash/Underscore but with lazy evaluation, which can translate to superior performance in many cases.

###Functional Javascript Books

- [Eloquent JavaScript](http://eloquentjavascript.net/) Has some chapters dedicated to functional programming. Read for free [online](http://eloquentjavascript.net/), or purchase a [paperback](http://www.amazon.com/gp/product/1593275846/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=1593275846&linkCode=as2&tag=marijhaver-20&linkId=VPXXXSRYC5COG5R5) copy.
- [Programming Javascript Applications : Robust Web Architecture with Node, HTML5, and Modern JS Libraries](http://www.amazon.com/Programming-JavaScript-Applications-Architecture-Libraries/dp/1491950293/ref=sr_1_1?s=books&ie=UTF8&qid=1426178193&sr=1-1&keywords=Eric+Elliot)
- [Professor Frisby's Mostly Adequate Guide to Functional Programming (in Javascript)](https://github.com/DrBoolean/mostly-adequate-guide)
- [Functional Programming in Javascript](http://www.amazon.com/Functional-Programming-JavaScript-Dan-Mantyla/dp/1784398225/ref=pd_sim_14_4?ie=UTF8&refRID=0TGVWR4T74JV8Q5RAVGY)

###Functional Programming Books, Papers & Articles

> Worthwhile publications on FP in languages other than Javascript.

- [Real World Haskell](http://book.realworldhaskell.org/)
- [Learn You a Haskell For Great Good](http://learnyouahaskell.com/)
- [Functional Programming in Javascript](http://www.amazon.com/Functional-Programming-JavaScript-Dan-Mantyla/dp/1784398225/ref=pd_sim_sbs_14_2?ie=UTF8&refRID=0VWN3N2HTT3XT9VPZFSB)
- [Game programming in Haskell](https://leanpub.com/gameinhaskell) Insights from a Haskell programmer on the challenges and rewards of building a game in Haskell
- [Functional Reactive Programming](http://manning.com/blackheath/)
- [Why Functional Programming Matters](http://www.cse.chalmers.se/~rjmh/Papers/whyfp.pdf) by John Hughes, 1984 #paper #pdf
- [Functional Programming in Swift](http://www.objc.io/books/) #iOS 
- [Living with Lambdas: Functional Programming in C++](https://pragprog.com/magazines/2013-07/living-with-lambdas)

###Articles to be Explored

> These are articles that were recommended for one reason or another, but I haven't actually read them to determine their status.

- [On the Importance of Purity](http://higherlogics.blogspot.pt/2007/10/on-importance-of-purity.html)
- [Total Functional Programming](http://www.eis.mdx.ac.uk/staffpages/dat/sblp1.pdf)
- [Swift Functional Programming Tutorial](http://www.raywenderlich.com/82599/swift-functional-programming-tutorial)
- [Functional Reactive React.js](https://medium.com/@garychambers108/functional-reactive-react-js-b04a8d97a540)
- [Reactive MVC and the Virtual DOM](http://futurice.com/blog/reactive-mvc-and-the-virtual-dom)
- [Curry or Partial Application?](https://medium.com/javascript-scene/curry-or-partial-application-8150044c78b8)
- [The General Theory of Reactivity](https://github.com/kriskowal/gtor) What is all this talk about reactive? Functional? Promises?

###Blogs to Follow

- [Lambda the Ultimate](http://lambda-the-ultimate.org/)
- [RisingStack Engineering](http://blog.risingstack.com/)

###Functional Languages -> Compile to Javascript

- [Elm-lang.org](http://elm-lang.org/)
- [ClosureScript](https://github.com/clojure/clojurescript) : A closure to JS compiler

###Functional UI

- [Functional UI and Components as Higher Order Functions](http://blog.risingstack.com/functional-ui-and-components-as-higher-order-functions/)

