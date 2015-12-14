# Variables

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
