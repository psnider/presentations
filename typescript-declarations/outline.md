# The Problems
## You want to use a 3rd-party Package, but it doesn't have the Declarations You Need
- it has type declarations, but not all of the ones you want
- it has type declarations, but you encounter an error that prevents you from writing your code
- it has type declarations, but they're incompatible with your module type
- it doesn't have type declarations at all

## Writing Good Declaration Files is Difficult
- Javascript is complex, so TypeScript must be complex, too
- There are multiple ways to express the same types
- Javascript package documentation is often unclear regarding types
- Scoping of declaration elements can be tricky
- Making declaration files compatible with different module systems is tricky
- It's hard to know what elements to *type* and what not to *type*
- Writing a declaration file leads to learning more about the package than you want to know

# Guidelines
- Follow the recommendations at DefinitelyTyped
- Study existing declarations for similarly shaped packages at DefinitelyTyped
- Use the names from the documentation whenever possible
- Carefully select type names that communicate their usage
- Use namespaces to keep your declarations out of the global scope
- Respect the methods for using a package: ambient and/or external
- Don't try to get package owners to incorporate TypeScript declarations
- packages change over time, including being renamed
- if you fix an existing type declaration, contribute your change back to the community  
   ...or pay a heavy "merge tax" during your subsequent updates

# Resources
- [existing type declarations](https://github.com/DefinitelyTyped/DefinitelyTyped)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/writing-declaration-files.html)  
  ~~but not [typescript.codeplex.com](https://typescript.codeplex.com/wikipage?title=Writing%20Definition%20%28.d.ts%29%20Files)~~
- [DefinitelyTyped](http://definitelytyped.org/guides/best-practices.html)
- [contributing to DefinitelyTyped](http://definitelytyped.org/guides/contributing.html)
- [TypeScript v1.8 Language Spec](https://github.com/Microsoft/TypeScript/blob/release-1.8/doc/spec.md)
- Solicit help from package authors, if unsure
- Solicit help on the [TypeScript IRC channel](http://webchat.freenode.net/?channels=typescript)


# Examples

| package or spec |  declaration | notes |
|-------------|--------------|-------|
| [tv4](https://www.npmjs.com/package/tv4) | [tv4 typings](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/tv4) |  |
| [imap](https://www.npmjs.com/package/imap) | [imap typings](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/imap) | [SO help](http://stackoverflow.com/questions/26249210/how-do-i-write-a-typescript-declaration-file-for-a-complex-external-commonjs-mod) |
| [nodemailer-pickup-transport](https://www.npmjs.com/package/nodemailer-pickup-transport) | [nodemailer-pickup-transport typings](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/master/nodemailer-pickup-transport) |  |
| [mailparser](https://www.npmjs.com/package/mailparser) | [mailparser typings](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/master/mailparser) | This package disappeared from DT at one point |
| [pino](https://www.npmjs.com/package/pino)  | [pino typings](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/pino) | [PR to DefinitelyTyped](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/9715),  [feedback from package author](https://github.com/mcollina/pino/issues/62) |
| [seneca](https://www.npmjs.com/package/seneca) | [seneca typings](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/seneca) | [help from package authors](https://github.com/senecajs/seneca/issues/159) |
| [GeoJSON](http://geojson.org/geojson-spec.html) | [GeoJSON typings](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/geojson) | emailed author |
| [component-emitter](https://www.npmjs.com/package/component-emitter) | [component-emitter typings](https://github.com/DefinitelyTyped/DefinitelyTyped/blob/master/component-emitter) |  |  |
| [node](https://nodejs.org/api/) | [node.js typings](https://github.com/DefinitelyTyped/DefinitelyTyped/blame/master/node/node.d.ts) |  |


# How to Submit your Type Declarations
- I recommend using [DefinitelyTyped PRs](http://definitelytyped.org/guides/pull-request.html) for now  
**tsd** and **typings** both use DefinitelyTyped  
The other systems are too new, and I prefer to wait for other people to fix the bleeding edge problems.  
- put your submissions on a branch named after the package name
