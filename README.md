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
* The usage of `count` is prohibited; we should use `sizeof` because it's more performant
* The usage of `create_function` is prohibited
* The usage of `print` is prohibited; we should use `echo` instead
* There is only one single space before and after an operator
* Line length should not exceed 120 symbols
* We should not use space after cast, for example, `(int)$var`
* We should not use space after not, for example, `!$foo`
* The maximum cyclomatic complexity is 30
* We should use early return approach to reduce the nesting
* No magic method of direct calls at all
* No unused arguments in the function signature
* No dead code import with use statement
* 

