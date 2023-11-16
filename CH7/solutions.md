1.re.compile()
2.They are oftenly used so that backslashes do have to be escaped
3.It'll return None if the regex pattern is not found in the string. If the pattern is found, the search() method returns a Match object
4.using the group() method
5.group 0 - coveres the entire match
  group 1 - covers the first parentheses set
  group 2 - covers the second parentheses set

6.Using a backslash, parentheses can be escaped
7.If there are no groups in the regex, the findall() method will return a list of string matches and if there are groups, itll return a list of tuples of strings
8.| is called a pipe and is used to match one of the many expressions
9.the ? signifies 2 things. 
   a)"match zero or one of the preceding group"
   b)signify nongreedy matching
10.+ - matches one or more
   * - matches zero or more
11.{3} will match 2 instnces of the preceeding group while {3,5} will match instances between 3 and 5
12.\d - Represents digit character
   \w - Represents digits, letters and the underscore
   \s - Represents space, tab or newline character
13.\D - represents any character that is NOT a digit from  0 to 9
   \W - represents any character that is NOT a letter, digit or a underscore
   \S - represents any character that is NOT a space, tab or a newline
14.(.*) stands for anything
   (.*?) usesd to match any text in a non-greedy fashion
15.[0-9a-z] or [a-z0-9]
16.passing re.IGNORECASE or re.I as a second argument to re.compile()
17.. matches all characters except the newline. When re.DOTALL is used, it matches newline as well
18.'X drummers, X pipers, five hens, X hens'
19.it allows you to add comments and whitespaces to the strings which are passses to re.compile()
20.re.compile(r'^\d{1,3}(,\d{3})*$')
21.re.compile(r'[A-Z][a-z]*\sNakamoto')
22.re.compile(r'(Alice|Bob|Carol)\s(eats|pets|throws)\s(apples|cats|baseballs).', re.IGNORECASE)
