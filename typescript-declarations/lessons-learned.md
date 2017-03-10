# Introductions
- What do you want to get out of tonight's presentation?
- How much TypeScript experience do you have?
- How much Node.js experience do you have?

## Questions
- What other languages do people use for servers?
- What other languages do people use for clients?


# Lessons Learned
**Setup**
- Setup can be difficult, so document it.  
(I've wanted to use GitHub's Boxen but haven't had time.)

**Complexity and Evolution**
- TypeScript is complex, because javascript is complex.  
- Sharing TypeScript between client and server is hard.  
You must use external modules, and much existing code uses internal modules.  
Angular2 is making things easier, as they use external modules too.
- Typescript is evolving quickly.  
So I'm always lagging behind in some part of the tech stack.
- Many people choose plain vanilla javascript instead.  
I've never felt comfortable with vanilla js.  
The argument is that small modules make types unnecessary.
- TypeScript isn't for everything:
  - Small scripts are fine without typing, such as grunt and gulp files and utilites.

**Specifying Types**
- Typing helps me use OSS libraries correctly
- Typing helps me communicate to users of my libraries
- I like dynamic types by default, with typing when helpful  
- importing modules can be confusing, due to its two forms: commonjs and es6
- I also like schemas for development.

**Declarations**
- Declarations are often complex.  
Sometimes 3rd-party declarations are wrong.  
- When you find an error in a declaration file that you use, repair it with a Pull Request.  
If you don't, you will create more work for yourself when you next setup the project.
- Managing dependencies can be difficult.  
TSD supported multiple versions.  
I think Typings does too, but I haven't learned the details.
- Managing declarations files is difficult.  
Recently, I've been upgrading from TSD to Typings
- Keep typings at the top directory.  
How to separate publishing type declaration files from TSD or Typings managed files?

**Build Management**
- Use tsconfig.json files to specify build configurations.
- Build using out-of-source-tree builds.  
Unfortunately, atom-typescript hasn't supported this yet.
- npm is your friend  
But publishing to npm is hard.
- Follow all npm guidelines: use semantic versioning, lower case filenames.
- Don't use global npm packages.  
These can cause version problems, and fight cloud deployments.

**Debugging and Testing**
- Use REPL, logging, and node-inspector for debugging.
- Use TypeScript for tests.
- I still don't have gulp setup correctly yet for monitoring file changes and rebuilding and redeploying

# Notes on organization
- Use text wherever possible  
  - text can be diffed in git
  - mermaid.js for diagrams
  - gfm for all docs
- manage sub-projects as subdirectories
