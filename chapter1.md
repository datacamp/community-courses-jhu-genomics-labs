---
title       : Genomic Data Science Specialization - Final Quiz Demo
description : This class provides an introduction to the Python programming language and the iPython notebook. This is the third course in the Genomic Big Data Science Specialization from Johns Hopkins University
attachments :
slides_link :

--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:781f7226ca
## Question 1

Write a Python program that takes as input a multi-FASTA file with DNA sequences, and computes the answers to the following questions. You can choose to write one program with multiple functions to answer these questions, or you can write several programs to address them. There will be a final quiz at the end of the Python for Genomic Data course that will require you to run this program on a provided multi-FASTA file. 

How many records are in the file? A record in a FASTA file is defined as a single-line header,  followed by lines of sequence data. The header of the record is distinguished from the sequence data by a greater-than (">") symbol in the first column. The word following the ">" symbol is the identifier of the sequence, and the rest of the line is the description.There should be no space between the ">" and the first letter of the identifier.

*** =instructions
- 14
- 740
- 1240
- 20
- 18
- 19
- 760

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Exactly! Keep up the great work."
test_mc(4, [msg_bad, msg_bad, msg_bad, msg_success, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:7187d6e84e
## Question 2

What are the length of the sequences in the file? What is the longest sequence and what is the shortest sequence? Are there more than one longest or shortest sequence? What are their identifiers?

What is the length of the longest sequence in the file?

*** =instructions
- 6007
- 3245
- 1247
- 10523
- 4510
- 4200

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(5, [msg_bad, msg_bad, msg_bad, msg_bad, msg_success, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:8f07414a65
## Question 3

In molecular biology, a reading frame is a way of dividing the DNA sequence of nucleotides into a set of consecutive, non-overlapping triplets. Depending on what nucleotide in the first triplet of the DNA sequence we start the reading frame, there are six possible reading frames - three in the forward (5' to 3') direction and three in the reverse (3' to 5'). For instance, the three possible forward reading frames for the sequence 
>``` AGGTGACACCGCAAGCCTTATATTAGC are: AGG∑TGA∑CAC∑CGC∑AAG∑CCT∑TAT∑ATT∑AGCA∑GGT∑GAC∑ACC∑GCA
∑AGC∑CTT∑ATA∑TTA∑GCAG∑GTG∑ACA∑CCG∑CAA∑GCC∑TTA∑TAT∑TAG∑C ```<

These are called reading frames 1,2, and 3 respectively. An open reading frame (ORF) is the part of a reading frame that has the potential to code for a protein or peptide. It starts with a start codon (ATG), and ends with a stop codon (TAA, TAG or TGA). For instance, ATGAAATAG is an ORF of length 9. Given an input forward reading frame (1,2, or 3) your program should be able to identify all ORFs present in each sequence of the FASTA file, and answer the following questions: what is the length of the longest ORF in the file? What is the identifier of the sequence containing the longest ORF? What is the starting position of the longest ORF in the sequence that contains it? The position should indicate the character number in the sequence. For instance, the following ORF in reading frame 1:
>sequence1
``` ATGCCCTAG ```
starts at position 1.
Note that although the following sequence:
>sequence2
``` ATGAAAAAA ```
doesn't have any stop codon in reading frame 1, we will not consider it to be an ORF in reading frame 1 because it doesn't end with a stop codon.

What is the length of the shortest sequence in the file?


*** =instructions
- 1081
- 257
- 475
- 132
- 834
- 1721

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(3, [msg_bad, msg_bad, msg_success, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:642d18896c
## Question 4

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:60978bf3e8
## Question 5

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:24d0be4fc4
## Question 6

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:53437f0648
## Question 7

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:ea1198f108
## Question 8

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:ed76e2e48e
## Question 9

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:9a3bc45efb
## Question 10

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:aad7d67a7a
## Question 10

Have a look at the plot that showed up in the viewer to the right. Which type of movies have the worst rating assigned to them?

*** =instructions
- Long movies, clearly
- Short movies, clearly
- Long movies, but the correlation seems weak
- Short movies, but the correlation seems weak

*** =hint
Hint Hint Hint

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

import pandas as pd
import matplotlib.pyplot as plt

```

*** =sct
```{r}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

msg_bad = "That is not correct!"
msg_success = "Great job! You are awesome."
test_mc(2, [msg_bad, msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:NormalExercise lang:python xp:100 skills:1 key:9d1e104368
## Regular Exercise

Do you remember the plot of the last exercise? Let's make an even cooler plot!

A dataset of movies, `movies`, is available in the workspace.

*** =instructions
- The first function, `np.unique()`, uses the `unique()` function of the `numpy` package to get integer values for the movie genres. You don't have to change this code, just have a look!
- Import `pyplot` in the `matplotlib` package. Set an alias for this import: `plt`.
- Use `plt.scatter()` to plot `movies.runtime` onto the x-axis, `movies.rating` onto the y-axis and use `ints` for the color of the dots. You should use the first and second positional argument, and the `c` keyword.
- Show the plot using `plt.show()`.

*** =hint
- You don't have to program anything for the first instruction, just take a look at the first line of code.
- Use `import ___ as ___` to import `matplotlib.pyplot` as `plt`.
- Use `plt.scatter(___, ___, c = ___)` for the third instruction.
- You'll always have to type in `plt.show()` to show the plot you created.

*** =pre_exercise_code
```{python}
import pandas as pd
movies = pd.read_csv("http://s3.amazonaws.com/assets.datacamp.com/course/introduction_to_r/movies.csv")

import numpy as np
```

*** =sample_code
```{python}
# Get integer values for genres
_, ints = np.unique(movies.genre, return_inverse = True)

# Import matplotlib.pyplot


# Make a scatter plot: runtime on  x-axis, rating on y-axis and set c to ints


# Show the plot

```

*** =solution
```{python}
# Get integer values for genres
_, ints = np.unique(movies.genre, return_inverse = True)

# Import matplotlib.pyplot
import matplotlib.pyplot as plt

# Make a scatter plot: runtime on  x-axis, rating on y-axis and set c to ints
plt.scatter(movies.runtime, movies.rating, c=ints)

# Show the plot
plt.show()
```

*** =sct
```{python}
# SCT written with pythonwhat: https://github.com/datacamp/pythonwhat/wiki

test_function("numpy.unique",
              not_called_msg = "Don't remove the call of `np.unique` to define `ints`.",
              incorrect_msg = "Don't change the call of `np.unique` to define `ints`.")

test_object("ints",
            undefined_msg = "Don't remove the definition of the predefined `ints` object.",
            incorrect_msg = "Don't change the definition of the predefined `ints` object.")

test_import("matplotlib.pyplot", same_as = True)

test_function("matplotlib.pyplot.scatter",
              incorrect_msg = "You didn't use `plt.scatter()` correctly, have another look at the instructions.")

test_function("matplotlib.pyplot.show")

success_msg("Great work!")
```
