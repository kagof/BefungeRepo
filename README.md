# BefungePower
Befunge-93 program using a recursive algorithm to generate x^n. Note that this appears to just return 0 for any value greater than 2^16-1. This is because the Befunge-93 stack is of 16-bit signed long integers.

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

The code in Befunge is:

    >   #x  #y                   v
    v "please enter x value: "   <
    >,,,,,,,,,,,,,,,,,,,,,,& 25*,  50 p v
    v "please enter n value: "          <
    >,,,,,,,,,,,,,,,,,,,,,,& 25*, :90 p v
                          v:            <
                     v %2:_v
                 v-1:_:2/               ^
                 >                      ^
         v  %2  _v#: <p091$<
         #       >    " :rewsnA",,,,,,,,90g.@
         >90g50g*90p ^
         |
         >90g:*90p   ^
