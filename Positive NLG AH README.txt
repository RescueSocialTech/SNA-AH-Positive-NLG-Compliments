* Social Rescue Tech example
** Positive NLG Compliments

[[./compliments.txt]]

*** Demonstrations
+ Video demonstration :: https://asciinema.org/a/w5ayuAEGGpgsxTCKWbAGRPfvZ

+ Video demonstration (mp4) :: [[./demo1.mp4]]

+ Video demonstration (gif) :: [[./demo1.gif]]

+ 8000+ and still generating :: https://asciinema.org/a/YexeaMmvc15iaGzHQFLMD1tr0

+ Video demonstration (mp4) :: [[./demo2.mp4]]

+ Video demonstration (gif) :: [[./demo2.gif]]

+ And still generating :: https://asciinema.org/a/cuCzjyq5EwT6dV8Xp3RIk9B3l

+ Video demonstration (mp4) :: [[./demo3.mp4]]

+ Video demonstration (gif) :: [[./demo3.gif]]

*** Code
+ Prompt :: http://github.com/semiosis/prompts/blob/master/prompts/compliment-generation-based-on-a-celebrity-1.prompt

*** Final generated prompt:
#+BEGIN_SRC text -n :async :results verbatim code
  The following are nice compliments:
  ###
  TOPIC: Jason Momoa
  - He has fame, but he doesn't want it. He has advantage but he doesn't take it. And he definitely has all our hearts!!!!!
  ###
  TOPIC: Amber Heard
  -
#+END_SRC

** Simulate real conversation using NLU and NLG
+ Demonstration :: https://semiosis.github.io/apostrophe/

+ Conversation demo 1 :: https://asciinema.org/a/K40px4H4CPPN15QMz6Uy8Pz3q

+ Video demonstration (mp4) :: [[./conv-demo1.mp4]]

+ Video demonstration (gif) :: [[./conv-demo1.gif]]

+ Conversation demo 2 :: https://asciinema.org/a/aLn5lZq5yIeBxR6dyFyveDJGc

+ Video demonstration (mp4) :: [[./conv-demo2.mp4]]

+ Video demonstration (gif) :: [[./conv-demo2.gif]]

+ Conversation demo 3 :: https://asciinema.org/a/YdX4bzPownHsVT3T0UPLMcp3c

+ Video demonstration (mp4) :: [[./conv-demo3.mp4]]

+ Video demonstration (gif) :: [[./conv-demo3.gif]]

** Time taken to generate
#+BEGIN_SRC bash -n :i bash :async :results verbatim code
  git show -s --format=%at a9fccf1
#+END_SRC

#+RESULTS:
#+begin_src bash
1639635963
#+end_src

#+BEGIN_SRC bash -n :i bash :async :results verbatim code
  git show -s --format=%at 08b7c56
#+END_SRC

#+RESULTS:
#+begin_src bash
1639627967
#+end_src

#+BEGIN_SRC bash -n :i bash :async :results verbatim code
  # Seconds
  echo "1639635963 - 1639627967" | bc
#+END_SRC

#+RESULTS:
#+begin_src bash
7996
#+end_src

#+BEGIN_SRC bash -n :i bash :async :results verbatim code
  # Total minutes
  echo "(1639635963 - 1639627967) / 60" | bc
#+END_SRC

#+RESULTS:
#+begin_src bash
133
#+end_src

It took just over 2 hours to generate 10k
compliments.

This pipeline will be sped up in the near future by a factor of around 10x.
