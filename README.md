# php-code-standard

Rules:

* We use tab `\t` for indentation
* No closing tag (`?>`) at the end of the file
* Each file has an empty new line at the end
* Bracket `{` should follow the same line of definition
* Bracket `[` should follow the same line of definition
* Multiline array declaration should contain`,` at the end of the last line
* Declaration of all functions should follow `underscore_style`
* Declaration of all method names of classes should follow `camelCaseStyle`
* **PHPStan** should run with the strictest level possible – `--level=9`
* No blank lines with spaces
* No spaces before or after function arguments (after `(` or before `)`)
* Strict equals only (for example, === or !==)
* We must use `'` over `"` all the time when there is no variable inside
* Always use the `"` without concatenation operator when we need to interpolate variables
* Each operator must be surrounded by spaces (for example, `$var = 'val'`)
* The usage of the `list` function is forbidden; we should use pattern matching instead
* The usage of `create_function` is prohibited
* The usage of `print` is prohibited; we should use `echo` instead
* There is only one single space before and after an operator
* Line length should not exceed 120 symbols
* We should not use space after cast, for example, `(int)$var`
* We should not use space after not, for example, `!$foo`
* The maximum cyclomatic complexity is 30
* The maximum cognitive complexity is 14
* We should use an early return approach to reduce the nesting
* No magic method of direct calls at all
* No unused arguments in the function signature
* No dead code import with a use statement
* No dead catches in try blocks
* No unused variables are  allowed
* No unused methods are allowed
* You should not use type in variable or any property name that you define
* `@` is forbidden to use in front of any function calls
* Use type casting instead of calling functions `strval` or `intval`
* Prefer the short ternary operator `?:` over the old one
* There should be no nested ternary operators on a single statement, only one level of nesting is allowed
* All variables should be named by using `camelCase` startingg with a non-capitalized letter
* All variables should be named in declarative format and without type prefix/suffix
* Repeated function calls in a cycle when unnecessary is prohibited
* Variable that contains flag/boolean should start with `is` or `has` a prefix to be more readable and understandable

## How to install hooks

You should download and install [pre-commit](https://pre-commit.com/) first. Once it's done you can go to the project dir where you want to activate git hooks and run the command:

```bash
pre-commit install
```

Please, remember that you should do it all the time once something updates in code style and it was deployed to the project.
