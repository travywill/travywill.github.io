---
layout: post
title:      "My First Major Ruby Project"
date:       2018-10-30 02:36:48 +0000
permalink:  my_first_major_ruby_project
---


Hello!

Welcome to my second blog post!  This post will discuss my experiences with my first student project for Flatiron School’s Online Full Stack Web Development Program.

My first project is a CLI Data Gem Portfolio Project.

Whoa … wait a sec!  That’s a mouthful!  What does that even mean?

Let’s break it down.

CLI stands for command-line interface.  Essentially, that refers to when the user interacts with the computer through textual commands (in contrast to clicking on icons or using menus).

Data refers to the fact that the project requires me to create a program that extracts data from one or more websites.

Gem is a term particular to the Ruby programming language and it refers to a Ruby program that is packaged in a way that makes it easy for other Ruby programmers to download and use.

For my project, I created a program that scrapes information off of www.goodreads.com that allows the user to enter search terms to look for books and then receive the first page of search results in a list format.  The user can then request to read a summary of one of those books if one piques their interest.  It’s a simple and fun program and one that’s great for a neophyte programmer (and bibliophile) such as myself.  I call it the GoodReads Book Gem.

The program primarily relies on three files in which I created three Ruby classes: Book, Scraper, and CLI.  Ruby allows programmers to create their own classes and objects.  Each object in a class shares certain characteristics with other objects in that class, but also has its own characteristics that make it unique.  For instance, objects in the Book class should each have a title, author(s), and a URL for its book profile webpage; however, these should be unique to each Book object (i.e. they should have unique titles, authors, and URLs).

My Book class is the simplest, with the three attributes listed above, along with an additional optional attribute that gives a summary of the book.  

The Scraper class is designed to scrape information off of a website, specifically off the GoodReads website.  It has two methods: the scrape_search_results method and the scrape_book_profile_page method.  In Ruby, a method is a set of instructions for the program that are bundled together so that they can be repeated in multiple places.  My scrape_search_results method has instructions to scrape the search results page on the GoodReads website to get certain information about each book listed in the results (i.e. the book’s title, author(s), and URL).  The scrape_book_profile_page method is designed to scrape the book’s profile page to retrieve the summary of the book.

My last class, the CLI class has a set of methods to direct the flow of the command-line interface, allowing the user to utilize the Book and Scraper classes to find information about books from the GoodReads website.

I’d say the most difficult part of this project was working on the Scraper class, particularly finding the right selectors to retrieve the relevant information from the HTML of the GoodReads website.  It took a quite a bit of time, effort and trial and error to discover the correct selectors and at times it was very frustrating.  Once I had solved this problem, writing the rest of the program was mostly smooth sailing.

Overall, I enjoyed working on this project.  It was particularly satisfying because it was one of the first computer programs I’ve written in Ruby that was completely my own design from start to finish.  While the program is relatively simple, I feel it represents a solid beginning for my web development career and I look forward to building on this foundation in future projects.

Best,

Travis (the Web Developer)

