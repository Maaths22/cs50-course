# Caesar code from CS50 Course.

#### Hello guys!

Giving the CS50 challenge to do the Plurality code, I've searched for some solutions but I saw a lot of them treating of new libraries and functions.
So I tried to do it differently, by starting with the input, and changing letter by letter using ASCII table.
There's nothing out of the box on it, because probably the functions other people used was developed like this, but I was happy to see it working, knowing that I went back coding this year.

#### So, what it does?
```
1 - The program will ask you a input right from the beggining, and it requests you to choose a positive integer and this will be used to build the cyphertext.

2 - With the number, the program asks you what is going to be you plaintext.

3 - By having those two inputs, the program processes the information to allow to do it using ASCII table:
  i) It holds the integer equivalent to the letter on your plaintext.
  ii) Adds to this the number informed at first time by running the program.
  iii)If this new number is bigger than the equivalency of lowercase z or uppercase Z, the program subtracts 26(nº of alphabetical letters). Else, it just print the respective letter of this integer.
  iv) It keeps doing this while the number isn't back to the lowercases or uppercases letters. So, it won't mess up by mixing small and capital letters.

4 - By the end, the user receives the output (i.e. the cyphertext).
```
So, as I said, there's nothing special on it, but I started coding again this year and that's my introduction to the GitHub community: the first code I've built from start to finish!
