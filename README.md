# Problem Set 10 (the last problem set!)

### Due Tuesday, May 4, 2021, at 11:59pm EST

As always, you will submit to Canvas **a single .zip file**. Detailed instructions for what the .zip file should contain are at the end of this problem set. 

Download this whole directory **to your desktop (!!!)**, unzip it, and carry out the tasks described below.

## Part 1: Using a Jupyter notebook

### Step 1: Installing jupyter
To use a Jupyter notebook, you need to install the `juypter` library. To do, just follow [the directions in PS7 for installing libraries](https://github.com/CSC1-1101-TTh9-S21/ps7#step-1-install-the-libraries). In other words, launch a Terminal (Mac) or command (Windows) and type:

`pip3 install jupyter`

Be sure to check the alternative things to type in [the previous instructions for installing libraries](https://github.com/CSC1-1101-TTh9-S21/ps7#step-1-install-the-libraries) in case you have an unusual configuration.

### Step 2: Opening the jupyter notebook
Keep your terminal open! You need to navigate to the folder you downloaded in order to access the jupyter notebook, `part1.ipynb`. Recall that your `ps10-main` folder you downloaded must be on your desktop in order for these instructions to work. Here is how to do it:

* On a Mac or in Linux, in a terminal type: 

```
cd ~/Desktop/ps10-main
jupyter notebook
```

* On Windows, in the command or cmd application, type the following:

```
cd Desktop 
```

If you get an error, try this instead, where `your-username` is your username.

```
cd c:\Users\your-username\Desktop
```

Then type

```
jupyter notbook
```

* On both Windows and Mac, this will open your default browser, and you'll see a screen that looks like this:

[INSERT SCREENSHOT HERE]

* Click on the file called `part1.ipynb`.

### Step 3: Using a jupyter notebook
Continue with the rest of Part 1 by following the instructions in the provided jupyter notebook, `part1.ipynb`.

## Part 2A (for people who will continue on to CS2)
**This component of the problem set is for students who plan to take CS2. If you do not plan to take CS2, you can skip this section.**

In this part, you will write a program that runs a simulation to approximate the best case, worst case, and average case for bubble sort and selection sort. Start by examining the files in the `part2A` folder. Open the included Python program, `part2A.py` in Atom. 

In `part2A.py`, you'll see that I have included the code for bubble sort and selection sort. 

* First, you will modify the code to keep track of and return the number of comparisons that are made in one run of the function. 

* Next, in your `main()` function, you will create two empty lists `bubblelist` and `selectionlist`. You will generate 100 different lists of length 10 of random integers. You will submit each list to the two sort methods and keep track of how many comparisons were required to sort each list. You will then report the minimum number of comparisons, the maximum number of comparisons, and the average number of comparisons for for each sorting algorithms. Finally, you will plot an appropriate labeled histogram for each list.

Below I have provided "pseudocode" for you to implement in your `main()` function:

```
declare bubblelist, selectionlist as empty lists
declare counter as an int equal to 0
while counter < 100
   create list of length 10 containing ten random integers between 1 and 100 (duplicates are okay)
   make a copy of that list
   submit the first list to bubblesort()
   append the result to bubblelist
   submit the second list fo selectionsort()
   append the result to selectionlist

print min, max, average of bubblelist
print min, max, average of selectionlist

create a plot with two subplots
plot histogram of bubblelist with appropriate labels
plot histogram of selectionlist with appropriate labels
```

* Finally, take a screenshot of your program in Atom and your output on the terminal so that I know you used Atom to write the program and the terminal to run the program.

## Part 2B (for people who will *not* continue on to CS2)
**This component of the problem set is for students who do *not* plan to take CS2. If you plan to take CS2, you can skip this section. If you are interested, you can complete part 2A, but you will be given no additional credit.**

In Part 2B you will be writing a program that lets you compare the frequencies of characters in four different languages and use this information to guess the language of a new input text. I have provided started code in the `part2B` directory in a file called `part2B.py`. Here are your tasks:

1. Write a function `countletters(filename)` that reads in a file (the argument `filename`) and counts the number of times each character appears in that file, storing this information in a dictionary that maps letters to frequencies in that file. The function will **return this dictionary**.

2. Inspect the code I have provided for the function called `plotdistributions(chardictionary)`, which takes as an argument one of the dictionaries you created above that maps letters to their counts in a text. This function will create a bar chart showing the distributions of the various characters in a text.

3. Write a function `predictlanguage(filename)` that calls `countletters(filename)` and then uses the output 

3. Take a screenshot of your program in the Anaconda editor and your output on the Anaconda Python shell so that I know you used Anaconda to write the program and the terminal to run the program.

---

## What to submit
 Delete `part2a.py` if you completed Part 2B. Delete the `part2b` folder if you completed Part 2A. 

When you have done this, you should have
 * a completed `part.ipynb`
 **AND** 
 * *EITHER* a completed `part2a.py` *OR* a `part2b` folder containing your completed `part2b.py` program and all the associated text files.
 
 
 Zip up the `ps10-main` folder, and submit the zipped file to Canvas.
 
 ### Due Tuesday, May 4, 2021, at 11:59pm EST




