# Programming from the Beginning

I've noticed throughout my computer science tutoring career that programming usually poorly taught.  The fundamentals are skipped through almost entirely - it's like trying to learn to play hockey without learning how to ice skate first.  They skip through explaining what something does and just have you copy and paste something you don't understand yet, thinking "oh, you'll get it.".  The students are led to believe that code is magic.

It's not.

Programming langauges are very exact, and there is no magic.  Every piece works the way it does for a reason.

I've created this tutorial to help people learn how programming actually works, starting from the beginning (what does this piece mean) rather than the end (paste this in and see if you can read it).

####Note on Macs:
You'll use Command key instead of the Control key.  Everywhere I say "CTRL", just use Command instead.



##Setting up Light Table

Download and run [Light Table](http://lighttable.com/).  This will vary depending on what OS (as in Windows, Mac, or Linux) you are using, but it will be as simple as downloading the file, unzipping it, and opening LightTable.

Looks like a nice, simple text editor, eh?  It has a lot of hidden power.  You can access all of the things it can do by pressing CTRL + SPACE.  It will open a drawer on the right side of the window where you can search all of the things the editor can do and use them.

Let's get things set up for Javascript.

- Make a new file. (CTRL + N)
- Set the *syntax* (language) of the file by pressing CTRL + SPACE and typing "syntax".  Select the action called "Editor: Set current editor syntax" and pick Javascript.
- Press CTRL + SHIFT + ENTER to run your empty file.  It will pop up with a message saying "No client available."
- Click "Connect a client".
- Click "Browser".  It should open up a blank white page.  For now, you can just switch back to our file by clicking it's tab on the top.

To run your work, you can use:

- CTRL + ENTER which runs only the line your cursor is on or whatever you have selected
- or CTRL + SHIFT + ENTER, which runs the entire file.

If it doesn't work, try connecting it to "Light Table UI" instead.

You're now ready to begin!

Sidenote: You are able to use Light Table for a lot of different languages in a similar way to how we're using it for Javascript.  You'll have to go to them for more information.



##A Comment About Comments

Comments are text inside code files that isn't run by the computer.

Writing comments how you keep notes on what your code means.  Without writing notes, it's easy to forget what a certain piece of code does.

Other people will probably read your code and comments too, so they should be written in plain, easy-to-read English.

They look like this:

    //This is a comment.

    Real code is here.  //However, this part is a comment.

    Here is some more code.

    //More comments!!

    /*This is a special type of comment
    that can be really long and
    go across many lines.*/

    More code!!

Anything that comes after // on a line is just a comment and the computer just ignores it.

Same thing goes for anything inbetween /\* and \*/.



##Learning about Expressions

Before you can really understand code, you need to understand what an "expression" is.

An expression is an instruction for the computer.  Bam, it's that simple.

Expressions can require inputs and usually have a result.  We call the inputs *arguments* or *parameters*, and we say that an expression *returns* the result.  So if I say that the expression *returns* something, it's result is that something.

You can see what an expression returns in Light Table by selecting it and pressing CTRL + ENTER.

There are lots of different things that are expressions.  Some expressions are just numbers, some do math, some put things on the screen, and some store information.  I'm going to teach you a lot of them.

We separate different expressions using semicolons (;), similar to how you would use periods to end a sentence in English.

Let me give you some examples.



##Our First Expressions: Numbers

Let's start with a really easy expression: a number.

Numbers take no inputs, and their result is themselves.

Here are some examples.  Try them one at a time.

    134;
    1;
    0;
    -42;  //You can use negatives.
    98.82;  //Decimals are OK.
    1.42e5; //"e" is for scientific notation.

Pretty easy, right?  You can try it out right now.  Put a number in your file on it's own line and press CTRL + ENTER.  A box with the number should show up right next to it.  That box is showing you the result of that expression.

That's not very helpful by itself though; it only gives back that we put in!  Let's look at another type of expression.



## The Plus Expression

A plus expression adds two numbers together.  It is structured like this:

    (firstNumber + secondNumber)

This is the first expression we've come across that uses inputs.  And those inputs are... expressions.  That's right, expressions inside expressions.  That's how all of programming is done.

Here are some examples using numbers for those expressions:

    (1 + 2);
    (53.2 + 95.5);
    (53 + -22);

But we can get trickier!

    ((42 + 12) + 24);

*We just put a plus expression inside a plus expression.*



## Other Math Expressions

You've probably guessed by now that you can also subtract, multiply, and divide.  Here's how those look:

    (firstNumber - secondNumber)
    (firstNumber * secondNumber)
    (firstNumber / secondNumber)

Some examples:

    (32 - 18);
    (5 * 8);
    (81 / 9);

    ((3 * 2) - 5);
    (5 * (3 / 2));
    (3 + (9 / 2));



## Less Parenthenses Please!

You don't need to use parenthenses around every piece of math, because the computer is smart.  It knows about [order of operations](http://www.purplemath.com/modules/orderops.htm) and can figure out what you mean.

Examples:

    3 * 2 + 4;
    4 + 5 - 6;

You can use this as a calculator now!  You can do a lot more than that though.



## Storage

You will frequently need to store information and then use it again.  Javascript has a simple way of doing this.  They are called *variables*.

### Setting aside a name
This is called *delcaring a variable*.

*This is a statement, and can't be used as an expression.*

    var name;

### Giving that name some information
This is called *assigning a variable* or *setting a variable*.

This is an expression, and it returns whatever it set name to.

The part on the right is always done first.

    name = expression;

This is most properly translated to English as "Set name to expression".  It's not really like equals, and the computer won't do algebra for you.

### Getting that information back
This expression returns the information you stored in it earlier.

    name;

### Short hand for declaring and assigning

    var name = expression;

### Some examples:

    var x;
    x = 22;

    var y = 43 - 29;

    x + 8;
    x + 2;

    x = y - 4;

    var z = x + y;
    z;

    x = x + 4;
    /*Seems odd, doesn't it?  But since the part on the right happens first,
    it takes the old "x" and adds 4 to it, then sets "x" to that new number.*/

    y = y * z;

Test them out and get used to them, because you'll be using them a lot.


## What About Words?

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
