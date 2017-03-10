March 3, 2017  
[Peter Snider](https://github.com/psnider)

# Why TypeScript?

First JavaScript, then TypeScript
> "It's mind-boggling difficult to work on large javascript projects."
- Anders-Hejlsberg

TypeScript annotates existing JavaScript with types, and supports converting to any common version of JavaScript.

So JavaScript is already valid TypeScript!


## Language Speed vs Expressiveness
- [Computer Language Benchmarks Game](http://benchmarksgame.alioth.debian.org/u64q/which-programs-are-fastest.html)
- [Guillaume Marceau: expressiveness and performance](http://blog.gmarceau.qc.ca/2009/05/speed-size-and-dependability-of.html)


## Language Popularity

Here are some indexes:
- [PYPL PopularitY of Programming Language](http://pypl.github.io/PYPL.html)
- [interactive graph based on engineers, classes, and vendors](http://www.tiobe.com/tiobe-index/)
- [The RedMonk Programming Language Rankings: June 2016](http://redmonk.com/sogrady/2016/07/20/language-rankings-6-16/)
- [JavaScript Is The Most Commonly Used Programming Language On Earth](https://arc.applause.com/2016/03/22/javascript-is-the-worlds-dominant-programming-language/)
- [Language Trends on GitHub](https://github.com/blog/2047-language-trends-on-github)

## My Language Selection Process
Here's a summary of what I understand about the most common languages, along with some of my opinions:

| language   | used for                 | speed | mem mgmt | difficulty | typing | libraries  | REPL  | OSS tools | like             | dislike |
|------------|--------------------------|-------|----------|------------|--------|------------|-------|-----------|------------------|---------|
| C/C++      | everything but web-pages | 100%  |          | hard       | strong, static | system |      | *nix, gdb | close to machine  | complex, memory mgmt, debugging |
| Java       | everything but web-pages, Android | 40-80%  | ✔ | easy | strong, static | :+1: | via groovy | eclipse | easy | JVM, threads, namespace model, debugging |
| Ruby       | scripts, servers | 10-60% | ✔ | moderate | strong, dynamic | :-1: | ✔ | eclipse | expressive, easy to read | threads, debugging |
| Python     | scripts, servers | 10-60% | ✔ | easy    | strong, dynamic, (static typing in 3.5)  | :-1: | ✔ | eclipse | expressive, easy to read | threads, debugging |
| JavaScript | everything | 10-50% | ✔ | hard | weak, dynamic  | :+1: | ✔ | Chrome debugger | expressive, naturally asynchronous, single-threaded, npm | complex, debugging |
| TypeScript | same as javascript | same as javascript | same as javascript | hard | optional strong static compile-time | same as javascript | ✔ | same as javascript + MSVS | same as javascript + typing | complex, debugging |


## Opinions about TypeScript
- [Angular: Why TypeScript?](https://vsavkin.com/writing-angular-2-in-typescript-1fa77c78d8e8#.tt4n5qrn3)
- [When should I use TypeScript?](https://medium.freecodecamp.com/when-should-i-use-typescript-311cb5fe801b#.6k7daqg2i)


# TypeScript Overview
- [TypeScript site](https://www.typescriptlang.org/)
- [TypeScript playground](http://www.typescriptlang.org/play/)



# Setup
Here are [the instructions I use to setup my MacBook laptop here](https://github.com/psnider/setup-mean-ts)

# TypeScript on Node.js
[TypeScript on Node.js](http://morning-savannah-8290.herokuapp.com/Typescript-on-Nodejs/presentation.html#/)


# A Micro-Service built using TypeScript for the Full Stack
[people-service](https://github.com/psnider/people-service)
