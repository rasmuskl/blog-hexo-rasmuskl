title: AlphaLaunch
date: 2013-10-11 23:27:27
categories: [AlphaLaunch]
---

Keyboard and search based interaction has always fascinated me. I've been an avid user of tools that enabled me to work faster and easier - and they've often been keyboard oriented and many of them have also featured powerful search. I've recently started to use some of my spare time experimenting with a small application launcher. The source code is not available at the moment, but I reckon I will throw it on Github soon. This post is meant as a rough outline of my thoughts on the subject.

# Examples

This kind of technology is already used in a ton of different projects and forms. 

There exists a ton of launchers for Windows with the most basic one probably being the start menu. Other examples include Launchy, FARR and Executor. My personal favorite for the past few years have been Launchy. Most of these are focused around the task of opening a file or launching a program, a single type of action, maybe with support for a few other action types as second class citizens through plugins. 

Interestingly the launchers that exist on Mac seem, from my limited research, to take a more holistic approach to performing whole actions on behalf of the user. This seems to be true for both Quicksilver, Alfred and Launchbar. The only thing I know of that resemble this on Windows is Enso, but it seems that most development died a few years back.

# Problem

The main problem that we're trying to solve with these 


- List of relatively short strings to filter down
- Capture user intent
- Indexing

# Goals / vision

- Performance
- Minimize user input to find desired item
- Incremental

- Context
- Action vs Launching
- Minimal syntax
- Learn / improve / boost
- Regex / Indexing / Ranking
- Performance / memory


# Types of search

There are multiple different kinds of search. The type of search that we're interested in is found in many applications these days and has quite a few names: Autocompletion, fuzzy search, incremental search, abbreviated search etc. This type of search is often based on a list of relatively short strings that is filtered down by various means - user input obviously and often also application context.


# Techniques

## Fuzzy string matching

String difference algorithms.

## Inverted indexes

Search in longer texts is usually based on words, often using an inverted index. This is what you get when you grab Lucene.NET from the shelf. As far as I understand, this is also roughly (simplified) how the web search engines work. While you can use these techniques for approximating autocompletion using tech like Lucene.NET's support for edge n-grams, I haven't been able to produce the quality of autocompletion that I'm interested in with.  

## Regular Expressions

- Everything / SwiftSearch

- Fuzzy search / exact / incremental / abbreviated search


# Other environments

- ReSharper, Sublime Text, TextMate
- Github / Bitbucket