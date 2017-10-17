# BefungeRepo:
This is a collection of fun little "programs" I've written in the [Befunge-93](http://esolangs.org/wiki/Befunge) esoteric programming language.

## List of Programs (in order of creation):
### [Power](https://github.com/kagof/BefungeRepo/blob/master/Power.bf)
Program using a recursive algorithm to generate x^n. This does not work for negative n.

The recursive algorithm used is:

    pow(x,n){
      if n==0 return 1
      
      else if n is odd {
        return x*pow(x,n-1)
       }
      else {
        return pow(x,n/2)*pow(x,n/2)
      }
    }

### [RunningEnd](https://github.com/kagof/BefungeRepo/blob/master/RunningEnd.bf)
An infinite loop in which the "end program" character '@' continuously runs away from the program counter.

### [NumberGuesser](https://github.com/kagof/BefungeRepo/blob/master/NumberGuesser.bf)
Asks the user to think of a number between 1 and 10, and guesses what the user is thinking of. This is a larger program, and the code is somewhat difficult to follow.

### [FizzBuzz](https://github.com/kagof/BefungeRepo/blob/master/FizzBuzz.bf)
Counts up from 1, saying "fizzbuzz" instead of multiples of 3 & 5, "fizz" instead of multiples of 3 & not 5, and "buzz" instead of multiples of 5 and not 3. I wanted to force myself to really use the 2-dimensional nature of Befunge, so I only allowed myself to write "fizzbuzz" once. Note that this is an infinite loop; be careful when running it!

### [Quine](https://github.com/kagof/BefungeRepo/blob/master/Quine.bf)
Program which outputs itself.

### [Factorial](https://github.com/kagof/BefungeRepo/blob/master/Factorial.bf)
Computes the factorial of the number input by the user.

### [PrimeGenerator](https://github.com/kagof/BefungeRepo/blob/master/PrimeGenerator.bf)
Quite inefficient program which lists all of the prime numbers (up to 2^16-1, to avoid potential arithmetic errors, and give the program a termination point). The counter compares each integer to ***every*** positive integer below it (excluding 1) to see if it is a divisor, hence it is definitely an incredibly inefficient algorithm.

### [HelloWorld](https://github.com/kagof/BefungeRepo/blob/master/HelloWorld.bf)
Hello world program in Befunge which never uses string mode to add characters to the stack. Prints "Hello world!" on the torus and to the output.
