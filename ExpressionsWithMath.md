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
