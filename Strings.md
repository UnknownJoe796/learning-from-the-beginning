# What About Words?

Numbers are one thing, but what about text?  In programming, text is usually called a *string*, which is short for a string of characters.  It can be empty or include spaces, letters, numbers and symbols.  They can be as long as you need them to be.

Examples:

    ""; //an empty string
    "Hello world!";
    " "; //a string with just a space in it
    "This is a longer set of words.  You can make strings a lot longer than one sentence.";

But what if the text is supposed to contain two lines, not just one?  And how would you use tabs?  What about a quote?  You can use these *escape sequences*.

| Code | Means          |
|------|----------------|
|\'	   |single quote    |
|\"	   |double quote    |
|\\\\  |backslash       |
|\n	   |new line        |
|\t	   |tab             |

Examples:

    "This is some text\non two lines";
    "\tThis is indented";
    "\\, \", and \' require backslashes to work";

Try some out yourself!



## Putting Words Together

Sometimes we want to take several strings and put them together.  That's called concatenation.  It's really easy to do; just add two strings together!

Example:

    "This " + "and that";

Even more, though, we can add a number to the end of a string using the same thing:

    "Current score: " + 8;
