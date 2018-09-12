# Ruby

## Tips
- (condition) ? (true_return_value) : (false_return_value)
- Case: <img width="615" alt="screen shot 2018-09-12 at 3 25 27 pm" src="https://user-images.githubusercontent.com/42748054/45448345-1b123200-b6a0-11e8-8f0d-b9c0b1a17216.png">

| code | use | 
|------|-----|
| # | comments | 
| =begin =end | multi line comments | 
| [variable] = [number]/[true/false]/"String | set variables |
| + - * / ** % | addition, subtraction, mult, division, exponentiation, modulo |
| puts | adds a new (blank line after the thing you want to print |
| print | prints to screen | 
| [string].length | return the length of the string (letters,numbers, spaces, symbols) |
| [string].reverse | returns the backwards version of the string you gave | 
| [string].upcase/downcase | returns ALL CAPS/lowercase |
| .to_s | converts number to a string |

# Formatting
## Spacing
- Use 2 space indent, no tabs.
- Use spaces around operators, after commas, colons and semicolons, around { and before }.
- No spaces after (, [ and before ], ).
- Avoid trailing whitespace.
- Indent when as deep as the case line.
- Use empty lines between method definitions and also to break up methods into logical paragraphs internally.
- End each file with a newline.

## Naming
- Use snake_case for symbols, methods and variables.
- Use snake_case for naming files and directories, e.g. hello_world.rb.
- The names of predicate methods (methods that return a boolean value) should end in a question mark (i.e. Array#empty?).  Methods that don’t return a boolean, shouldn’t end in a question mark.
Method names should not be prefixed with is_. E.g. prefer empty? over is_empty?.
- Never start a method with get_.
- Never use a ! at the end of a method name if you have no equivalent method without the bang. Methods are expected to change internal object state; you don’t need a bang for that. Bangs are to mark a more dangerous version of a method, e.g. save returns a bool in ActiveRecord, whereas save! will throw an exception on failure.

## Strings
- Prefer string interpolation and string formatting instead of string concatenation:   
_bad_    
email_with_name = user.name + ' <' + user.email + '>'     
_good_     
email_with_name = "#{user.name} <#{user.email}>"   
_good_   
email_with_name = format('%s <%s>', user.name, user.email)

- With interpolated expressions, there should be no padded-spacing inside the braces.   
_bad_      
"From: #{ user.first_name }, #{ user.last_name }"   
_good_      
"From: #{user.first_name}, #{user.last_name}"   
- Adopt a consistent string literal quoting style.
- Don’t use Object#to_s on interpolated objects. It’s invoked on them automatically.   
_bad_     
message = "This is the #{result.to_s}."   
_good_   
message = "This is the #{result}."
- Use %()(it’s a shorthand for %Q) for single-line strings which require both interpolation and embedded double-quotes.
- Avoid %q unless you have a string with both ' and " in it. Regular string literals are more readable and should be preferred unless a lot of characters would have to be escaped in them.
- Avoid the use of %s. Use :"some string" to create a symbol with spaces in it.

## Conditional Statements
- Use ! instead of not.
- Prefer &&/|| over and/or. More info on and/or for control flow (Links to an external site.)Links to an external site..
- Favour the ternary operator(?:) over if/then/else/end constructs.
- Use one expression per branch in a ternary operator. This also means that ternary operators must not be nested. Prefer if/else constructs in these cases.
- Use when x then ... for one-line cases.
- Favour unless over if for negative conditions.
- Do not use unless with else. Rewrite these with the positive case first.
## Methods
- Use def with parentheses when there are parameters. Omit the parentheses when the method doesn’t accept any parameters.
