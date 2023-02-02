# Collaborating with Git

Your task is to work in a pair to practice using git.

## Setup

1. One of you will need to _fork_ this repo to their own account.
2. In the forked repo, go to 'Settings -> Manage Access -> Invite People' and add person 2's github account as a collaborator
3. Then you can both make a local copy of the repo by running `git clone <link-to-pair-1s-forked-repo-here>`. (Remember to `cd` into the repo!)

You are now ready to start the challenges.

## Challenges

### Person 1

1. Using the terminal create a new file called `git-terminology.txt` and add the snippet below to the file:

```txt
git clone <github-link-here> - makes a local copy of the remote repo at the specified link
git status - shows the state of files in our working directory and staging area
git add <file-name> - adds a file from the working directory to the staging area
git commit -m "<message-here>" - makes a commit including all changes in the staging area
```

_Hint: Think about what happens when you use double-quotes to wrap a string that contains double quotes!_

2. Make a new commit to include this change
3. Push this new change up to github

At this point, press refresh on the github page - you should be able to see the newly added file.

### Person 2

4. Pull your pair's changes down from github to your locally cloned repo
5. Now that you also have the `git-terminology.txt`, add the definitions below:

```txt
git log - shows the most recent commits
git push origin main - pushes any recent, locally made commits to the remote repo ('origin') on the main branch
git pull origin main - brings any recent changes to the remote repo's main branch into your local repo
```

6. Create another file called `fun-facts.txt` and add your favourite colour to it.
7. Make commits to include your new changes - _remember_ if you need to write 'and' in the commit message then they should be separate commits.
8. Push your new commits up to github.

Again, press refresh on the github page - you should be able to see the new changes.

### Person 1

9. Pull down the most recent commits.
10. Add your favourite colour to `fun-facts.txt` and commit this change
11. Push up your changes to github

## Command Line Tasks

### Motivation

The objective of this small collection of tasks is to get you familiarised with some of the very powerful command line utilities available to you. This site is a [good source of documentation.](http://oliverelliott.org/article/computing/ref_unix/). Remember to look carefully throughout the first 20 commands to see if any of them will be useful. You should be able to complete all of these tasks with pure command line magic.

For each of the tasks below you can use the redirect operator `>` in order to generate a `.txt` file after running a command.

You should continue to follow pair programming practices during these tasks. Please remember to swap roles regularly!

Good luck 😄

### Tasks

1. Create a file called `first_10_words.txt` with the first 10 words from the word_list. Research the `head` command for this one.

2. Create a file called `last_10_words.txt` with the last 10 words from `word_list`.

3. Create a file called `word_count.txt` containing a count of all the words in the `word_list`.

4. Create a file called the `reversed_words.txt` with all the of the words from `word_list` but in reverse order.

**Note** - now may be a good time to swap driver/navigator roles!

5. Create a file called `3_or_more_vowels.txt` featuring all the words in the list that contain 3 or more vowels.
   Research `grep` or `egrep` for this problem.

6. Create a file called `b--.txt` with all the words starting with the letter b and ending in exactly 2 vowels.

7. Create a file consisting of all the 2 letters words. Store them in a file called `2_letters_only.txt`

8. Create a file containing a count of all the words starting with p to all the words starting with r - store the count in a file called `p_to_r.txt`. **Add** a word count to the end of the `p_to_r.txt` with a word count for the file.

## Advanced

Well done if you've got this far! 🎉

Here are a few extra tasks to help you get used to some of the JavaScript tools we will be using during the rest of this week and beyond!

In the `advanced.js` file we have imported in an array containing a list of words. Do not worry about how we've imported this in, it's something that will be covered later this week.

The objective is to practice solving some similar problems to the ones from the previous command line section using JavaScript instead.

You should not make any changes to the array within the file, any code you write should be below line 13.

If you need any tips about how to tackle these tasks, please refer to our good friend, [MDN](https://developer.mozilla.org/en-US/)

### Tasks

Each time you create a variable to solve one of these tasks, please `console.log` that variable to ensure the task has been correctly solved.

To see the console.logs, run the file by typing `node advanced.js` in your terminal. Please ensure you are in the correct file directory by making use of `pwd`.

1. Create a variable called `firstThreeWords` which contains the first three words in the list.

2. Create a variable called `lastThreeWords` which contains the last three words in the list.

3. Create a variable called `wordCount` which lets us know how many words are in the list.

4. Create a variable called `twoLetterWords` consisting of all the two letter words in the list.

5. Create a variable called `longestWord` which contains the longest word in the list.

6. Create a variable called `containsC` which contains all the words containing the letter C.

7. Create a variable called `reversedWords` which contains the list of words in reverse order.

**HINT - For this next section, a really useful tool to look into is RegEx, please check out this fantastic resource here - [RegExr](https://regexr.com/)**

8. Create a variable called `noVowels` which contains a list of all the words containing no vowels.

9. Create a variable called `repeatedLetters` which contains all of the words containing repeated letters.
