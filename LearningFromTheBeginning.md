# Programming from the Beginning

I've noticed throughout my tutoring career that programming usually poorly taught.  They skip through explaining what something does and just have you copy and paste you don't understand yet, thinking "oh, you'll get it.".  They try to explain it like it's a human language.

It's not.

Programming langauges are very exact, and there is no magic behind their format.  Every piece works the way it does for a reason.

I've created this tutorial to help people learn how programming actually works, starting from the beginning (what does this piece mean) rather than the end (paste this in and see if you can read it).

####Note on those darn Macs:
You'll use Command key instead of the Control key.  Everywhere I say "CTRL", just use Command instead.



##Setting up Light Table

Download and run [Light Table](http://lighttable.com/).  This will vary depending on what OS (as in Windows, Mac, or Linux) you are using, but it will be as simple as downloading the zipped file, unzipping it, and clicking LightTable.

Looks like a nice, simple text editor, eh?  It also has a lot of hidden power.  You can access all of the things it can do by pressing CTRL + SPACE.  It will open a drawer on the right side of the window where you can search all of the things the editor can do and use them.

Let's get things set up for Javascript.

- Make a new file. (CTRL + N)
- Set the *syntax* (a.k.a. language) of the file by pressing CTRL + SPACE and typing "syntax".  Select the action called "Editor: Set current editor syntax" and pick Javascript.
- Press CTRL + SHIFT + ENTER to run your empty file.  It will pop up with a message saying "No client available."
- Click "Connect a client".
- Click "Browser".  It should open up a blank white page.  For now, you can just switch back to our file by clicking it's tab on the top.

To run your work, you can use:

- CTRL + ENTER which runs only the line your cursor is on or whatever you have selected
- or CTRL + SHIFT + ENTER, which runs the entire file.

You're now ready to begin!

Sidenote: You are able to use Light Table for a lot of different languages in a similar way to how we're using it for Javascript.  You'll have to go to them for more information.



##Learning about Expressions

Before we can really understand code, we need to understand what an "expression" is.

An expression is an instruction for the computer.  Bam, it's that simple.

Expressions can require *inputs* and usually have a *result*.

There are lots of different things that are expressions.  Some expressions are just numbers, some do math, some put things on the screen, and some store information.

We separate different expressions using semicolons (;), similar to how you would use periods to end a sentence in English.

Let me give you some examples.



##Our First Expression: Numbers

Let's start with a really easy expression: a number.

Numbers take no inputs, and their result is themselves.

Here are some examples.  Try them one at a time.

    134;
    1;
    0;
    -42;
    98.82;
    1.42e5;

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

    (firstNumber - secondNumber);
    (firstNumber * secondNumber);
    (firstNumber / secondNumber);

Some examples:

    (32 - 18);
    (5 * 8);
    (81 / 9);

    ((3 * 2) - 5);
    (5 * (3 / 2));
    (3 + (9 / 2));



## Less Parenthenses Please!

You don't need to use parenthenses around every piece of math, because the computer is smart.  It knows about [order of operations](http://www.purplemath.com/modules/orderops.htm) and can figure out what you mean.

Example:

    3 * 2 + 4;
    4 + 5 - 6;

You can use this as a calculator now!  You can do a lot more than that though.



##A Comment About Comments

Comments are writing inside code files that isn't run by the computer.

That's how you keep notes on what your code means.  Without writing notes about it, it's easy to forget what a certain piece does.

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
