##Functional Programming Resources

This resource is meant to serve as an archive of the best resources surrounding the functional programming paradigm.

Functional programming is making a strong comeback, and with it: a massive wave of internet buzz. Someone needs to sort the good from the bad, and that is what I will attempt to do here.
My focus is on the functional paradigm in the context of Javascript, but discussion and highlight of other Functional languages are welcome for the purpose of evaluation, comparison and education.

###Articles

- **[Functional Programming for the Rest of Us](http://www.defmacro.org/ramblings/fp.html).** This article has a really great way of explaining some of the heavier aspects of FP. It breaks out of the typically-academic approach; speaking directly to developers, and not an assembly of mathematicians.

###Benefits of Functional Programming

- **Unit Testing** No function can ever cause side-effects, there is no need to care about external state, or calling functions in any particular order, all you need to do is pass arguments to your functions that represent your edge cases, this makes unit testing *an absolute dream*, and your applications can ship with confidence!
- **Debugging** Debugging a functional program is a breeze. If a function doesn't behave appropriately, just take a peek at your stack, and all the functions and variables that lead you to this point are staring right at you. No need to examine any external state, or investigate who/what/where could have interfered, it's all right in front of you.
- **Concurrency** The functional programming paradigms offers concurrency as a bonus right out of the box. Nothing in a functional program is ever modified twice by the same thread, let alone by two different threads. There is never any need to use locks, or worry about race conditions. Add as many threads to your app as you want, and your program will keep humming away. Beautiful.
- **Hot Code Deployment** Ever wish you could update/patch your live application without having to shut the system down first? With FP, it's not a problem!
- **Machine-Assisted Proofs & Optimizations** Because functional languages share a common root in mathematics, tooling for optimizations, testing, evaluation, etc can be built to further demonstrate the validity of your application. See "[Machine Assisted Proofs and Optimizations](http://www.defmacro.org/ramblings/fp.html)" for more information.
- **Highly-Readable Code** FP is an extremely expressive design paradigm, and this expressiveness tends to lend itself to beautifully-crafted programs that are clear and concise.
- **Excellent Code Reuse** The FP paradigm supports modular, reusable code straight out of the box. This is because functions compose themselves of existing functions, so you get to decide how these functions are combined to perform your application logic.
- **Highly-Maintainable Code** FP programs are incredibly easy to read, due to the declarative (and modular) nature of functional programming. Additionally: Functional programs also tend to be shorter than their imperative counterparts, and a smaller code base is easier to maintain than a large one.

###Libraries & Frameworks
- [functionaljs](http://functionaljs.com/)** A functional JavaScript library. It facilitates currying and point-free / tacit programming and this methodology has been adhered to from the ground up.
- [immuateble.js](https://github.com/facebook/immutable-js) Not entirely-functional, but shares a lot of the same concepts with functional design, namely the immutability of data.

###Books

- [Eloquent JavaScript](http://eloquentjavascript.net/) Has some chapters dedicated to functional programming. Read for free [online](http://eloquentjavascript.net/), or purchase a [paperback](http://www.amazon.com/gp/product/1593275846/ref=as_li_qf_sp_asin_il_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=1593275846&linkCode=as2&tag=marijhaver-20&linkId=VPXXXSRYC5COG5R5) copy.
- [Programming Javascript Applications : Robust Web Architecture with Node, HTML5, and Modern JS Libraries](http://www.amazon.com/Programming-JavaScript-Applications-Architecture-Libraries/dp/1491950293/ref=sr_1_1?s=books&ie=UTF8&qid=1426178193&sr=1-1&keywords=Eric+Elliot)

###Articles to be Explored
These are articles that were recommended for one reason or another, but I haven't actually read them to determine their status. Could be that some of these articles are too academic for my tastes.

-[On the Importance of Purity](http://higherlogics.blogspot.pt/2007/10/on-importance-of-purity.html)
-[Total Functional Programming](http://www.eis.mdx.ac.uk/staffpages/dat/sblp1.pdf)

###Blogs to Follow
-[Lambda the Ultimate](http://lambda-the-ultimate.org/)