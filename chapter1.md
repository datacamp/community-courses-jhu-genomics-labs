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
>``` AGGTGACACCGCAAGCCTTATATTAGC are: AGG∑TGA∑CAC∑CGC∑AAG∑CCT∑
TAT∑ATT∑AGCA∑GGT∑GAC∑
ACC∑GCA∑AGC∑CTT∑ATA∑
TTA∑GCAG∑GTG∑ACA∑CCG∑
CAA∑GCC∑TTA∑TAT∑TAG∑C ```

These are called reading frames 1,2, and 3 respectively. An open reading frame (ORF) is the part of a reading frame that has the potential to code for a protein or peptide. It starts with a start codon (ATG), and ends with a stop codon (TAA, TAG or TGA). For instance, ATGAAATAG is an ORF of length 9. Given an input forward reading frame (1,2, or 3) your program should be able to identify all ORFs present in each sequence of the FASTA file, and answer the following questions: what is the length of the longest ORF in the file? What is the identifier of the sequence containing the longest ORF? What is the starting position of the longest ORF in the sequence that contains it? The position should indicate the character number in the sequence. For instance, the following ORF in reading frame 1:
>sequence1
```ATGCCCTAG```
<p>starts at position 1.
<p>Note that although the following sequence:
>sequence2
```ATGAAAAAA```
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
A repeat is a substring of the DNA sequence that occurs in multiple copies (more than one) throughout the sequence. Although repeats can occur on both forward or reverse strand of the DNA sequence, we will only consider repeats on the forward strand here. 

Also we will assume that the repeats can overlap. For instance the sequence ACACA contains two repeats of length 3: ACA amd CAC. CAC occurs while once in the sequence at position 2 (index 1 in Python), while ACA occurs twice - once at position 1, and once at position 3. 

Given a length n, your program should be able to identify all the repeats of length n in all sequences in the FASTA file. Your program should also find out how many times each repeat occurs in the file, and which is the most frequent repeat of a given length.

What is the length of the longest ORF appearing in reading frame 2 of any of the sequences?
1. 1488
_2_.1134
3. 1518
4. 834
5. 1271
6. 1272

*** =instructions
- 1488
- 1134
- 1518
- 834
- 1271
- 1272

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
5:
* At what position in the sequence starts the longest ORF in reading frame 3? The position should indicate the character number in the sequence. For instance, the following ORF:
> sequence1
ATGCCCTAG
starts at position 1.
1. 237
2. 1045
_3_. 1818
4. 39
5. 575
6. 2100



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
6:
* What is the length of the longest ORF appearing in any sequence and in any forward reading frame?
_1_. 1518
2. 1488
3. 1095
4. 834
5. 1272
6. 2712


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
7.
* What is the length of the longest ORF that appears in the sequence with the identifier  gi|142022655|gb|EQ086233.1|97?
1. 2067  
2. 1551
3. 1358
_4_. 1272
5. 1080
6.783
7.588



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
8.
* What is the most number of times the most frequent repeat of length 6 appears in all sequences?
1. 153
_2_. 158
3. 72
4. 541
5. 98
6. 356


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

How many repeats of length 12 have the largest number of occurences in all the sequences?

*** =instructions
- 3
- 1
- 7
- 24
- 9

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
test_mc(1, [msg_success, msg_bad, msg_bad, msg_bad, msg_bad])
```
--- type:MultipleChoiceExercise lang:python xp:50 skills:1 key:9a3bc45efb
## Question 10
10:
Which one of the following repeats of length 7 has a maximum number of occurences?


*** =instructions
- CGGCGGC
- CGGCGCT
- TGGTGGC
- GCCGCCG
- GCGGCGC
- TCGGCGC

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
test_mc(1, [msg_success, msg_bad, msg_bad, msg_bad, msg_bad, msg_bad])
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
