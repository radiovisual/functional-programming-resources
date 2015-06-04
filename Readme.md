##Functional Programming Resources

An archive of the best resources surrounding the functional programming paradigm.

Functional programming is making a strong comeback, and with it: a massive wave of internet buzz. Someone needs to sort the good from the bad, and that is what I will attempt to do here.
My focus is on the functional paradigm in the context of Javascript and Swift, but discussion and highlight of other Functional languages are welcome for the purpose of evaluation, comparison and education.

**Note:** this is very much a work in progress!

###Keywords

- **Higher-Order Functions** A fancy term for a function that accepts another function as an argument. *[source](http://www.quora.com/What-is-a-simple-explanation-of-higher-order-functions-and-callbacks-in-JavaScript)*
- **Currying** Currying is the process of transforming a function that takes multiple arguments into a function that takes just a single argument and returns another function if any arguments are still needed. *[source](http://tech.pro/tutorial/2011/functional-javascript-part-4-function-currying)*
- **Pure Functions** A pure function is a function that does not introduce and "side effects" by affecting state anywhere in your application. Pure functions return a value, and that is all they do. This keeps your functions clean, predictable, and highly-testable.
- **Functors** A class type that can be mapped over with a function. A functor is a wrapper that can apply a given function to its contents & return a new instance containing the results. e.g. JS Arrays.
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

###Videos & Presentations

- [Simple Made Easy](http://www.infoq.com/presentations/Simple-Made-Easy) by Rich Hickney (author of Clojure)
- [React.js Conf 2015 - Immutable Data and React](https://www.youtube.com/watch?v=I7IdS-PbEgI) Not 100% about FP, but has some great tips on immutable data with the react.js library.

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
- **Variables are not immutable in Javascript.** Certain libraries / frameworks exist to help shape Javascript variables into immutable symbols. Note that the `const` keyword is coming to ES6, and has limited support right now.

###Libraries & Frameworks

- [Ramda](http://ramdajs.com/) A practical functional library for Javascript programmers. See [this article](http://developer.telerik.com/featured/practical-functional-javascript-ramda/) for a nice introduction. Some good functional nuggets to be enjoyed.
- [functionaljs](http://functionaljs.com/) A functional JavaScript library. It facilitates currying and point-free / tacit programming and this methodology has been adhered to from the ground up.
- [immutable.js](https://github.com/facebook/immutable-js) Not entirely-functional, but shares a lot of the same concepts with functional design, namely the immutability of data.

###Functional Javascript Books

- [Eloquent JavaScript](http://eloquentjavascript.net/) Has some chapters dedicated to functional programming. Read for free [online](http://eloquentjavascript.net/), or purchase a [paperback](http://www.amazon.com/gp/product/1593275846/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=1593275846&linkCode=as2&tag=marijhaver-20&linkId=VPXXXSRYC5COG5R5) copy.
- [Programming Javascript Applications : Robust Web Architecture with Node, HTML5, and Modern JS Libraries](http://www.amazon.com/Programming-JavaScript-Applications-Architecture-Libraries/dp/1491950293/ref=sr_1_1?s=books&ie=UTF8&qid=1426178193&sr=1-1&keywords=Eric+Elliot)

###Functional Swift Books

- [Functional Programming in Swift](http://www.objc.io/books/)

###Functional Swift Videos

- [Functional Programming in Swift](https://realm.io/news/functional-programming-swift-chris-eidhof/)

###Functional Programming Books

- [Real World Haskell](http://book.realworldhaskell.org/)
- [Learn You a Haskell For Great Good](http://learnyouahaskell.com/)
- [Functional Programming in Javascript](http://www.amazon.com/Functional-Programming-JavaScript-Dan-Mantyla/dp/1784398225/ref=pd_sim_sbs_14_2?ie=UTF8&refRID=0VWN3N2HTT3XT9VPZFSB)

###Articles to be Explored
These are articles that were recommended for one reason or another, but I haven't actually read them to determine their status. Could be that some of these articles are too academic for my tastes.

- [On the Importance of Purity](http://higherlogics.blogspot.pt/2007/10/on-importance-of-purity.html)
- [Total Functional Programming](http://www.eis.mdx.ac.uk/staffpages/dat/sblp1.pdf)
- [Swift Functional Programming Tutorial](http://www.raywenderlich.com/82599/swift-functional-programming-tutorial)
- [Functional Reactive React.js](https://medium.com/@garychambers108/functional-reactive-react-js-b04a8d97a540)
- [Reactive MVC and the Virtual DOM](http://futurice.com/blog/reactive-mvc-and-the-virtual-dom)


###Blogs to Follow
- [Lambda the Ultimate](http://lambda-the-ultimate.org/)
- [RisingStack Engineering](http://blog.risingstack.com/)

###Functional Languages -> Compile to Javascript

- [Elm-lang.org](http://elm-lang.org/)
- [ClosureScript](https://github.com/clojure/clojurescript) : A closure to JS compiler

###Functional UI

- [Functional UI and Components as Higher Order Functions](http://blog.risingstack.com/functional-ui-and-components-as-higher-order-functions/)

