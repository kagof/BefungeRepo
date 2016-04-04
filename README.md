# BefungeRepo:
This is a collection of fun little "programs" I've written in the [Befunge-93](http://esolangs.org/wiki/Befunge) esoteric programming language.

## List of Programs:
### Power
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

### RunningEnd
An infinite loop in which the "end program" character '@' continuously runs away from the program counter.
