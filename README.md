# Crafting-Interpreters
A repository to store the code for crafting interpreters as I work through the book.

## Getting Started ##
In order to build and run the **app** project you will need to first run the 'generateAst' task in the utilities project so that the AST classes are generated and can be consumed by the main (app) project. This can be done like so.

`gradle :utilities:generateAst`

Once that is done, you can then run the interpreter by using the run command to run the **app** project. 

**Note:** make sure to use the -q flag and the plain console option, or gradle will show the interactive logging which will mangle the output of the interpretor and make it harder to read.

`./gradlew run -q --console=plain`

## Quick Reference ##
- `gradle init` - initializes a new gradle project
- `gradle --version` - shows the current gradle version
- `./gradlew build` - Builds a gradle project
- `./gradlew run` - Runs a gradle project 
- `./gradlew` run -q --console=plain - Runs the gradle project in quiet mode and with no console logging (useful for command line applications that read from stdin)

- `gradle :utilities:generateAst` - Run the generateAst task for the utilities sub project
