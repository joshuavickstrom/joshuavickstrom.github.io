---
layout: post
title:      "Command-line Interface (CLI) Ruby Gem Project"
date:       2018-01-29 17:43:32 +0000
permalink:  command-line_interface_cli_ruby_gem_project
---


I’ve just finished the first portfolio project for Flatiron’s Full Stack Web Development program and I couldn’t feel more proud! 

Initially, just the idea of starting the project was somewhat daunting. After reading through each task the project requires, I began to construct a timeline to structure myself for success. Once the timeline was complete, I began working on the first task: coding the gem. I had participated in a Flatiron study group that demonstrated how to use an Application Program Interface (API) rather than scraping information off the web. I chose to use an API instead of scraping because I wanted to reduce the number of potential updates, should the website make changes that would impact my gem. However, I had never coded with an API before, so I set out to discover more (helpful resources linked at the bottom).  
Feeling empowered that I knew exactly how to tackle my gem (at least, in theory) I searched the internet for a decent API to use. Eventually, I found the BreweryDataBase (despite my own distaste for beers) and decided it was the right fit. I read up on the documentation provided and made the following outline for the CLI:
      •	Welcome user and provide instructions (“Please provide a US state to receive a list of breweries in that region.”) 
      •	Access API using user input
      •	Puts numbered list of breweries for provided region (just names)
      •	Provide instructions for next steps (“Please provide the number corresponding to the name of a brewery you would like more information about.)
      •	Gets user input and puts “pretty” menu providing brewery name, address, and website
      •	Ask if the user wanted to search another region, or to quit
      •	Exit program if user wants, else restart from the beginning 
The first challenge I faced when coding this gem involved accessing the data I had identified as necessary for my gem. I was over-thinking the code and wasn’t attending to the information I had collected from online resources. It took me several tries, over the course of one day, but finally my brain synapsed, and I realized how similar using an API was to scraping! I succeeded in instantiating objects for brewery names, addresses (formatted properly for navigation), and websites (but I had to tackle the issue of breweries that did not have a site! More on that later). 
The second challenge I faced involved using the instantiated objects to puts out specific brewery information. For some reason, I had simply forgotten to interpolate the data I had taken from the database, shoveled into the @@all array, and had waiting patiently to be accessed. So, after trying some different methods iterations, I turned again to Google and was reminded of the basic, fundamental principle of interpolation! 
Small challenges that were fun to code through included: Booleans to check user inputs whenever the gem required input and coding helper methods to “cleanup” my code. 
Overall, I’d say this project was a blast and I can’t wait to develop my own gems, just for fun! 

For anyone who made a similar decision to use API vs scraping, I found the following resources to be helpful, but they only pertain to the Ruby language: 
•	[FreeCodeCamp](http://https://medium.freecodecamp.org/what-is-an-api-in-english-please-b880a3214a82) 
•	[CodeAcademy](http:/https://www.codecademy.com/courses/ruby-beginner-en-pEdhY/0/1?curriculum_id=5122d839c0a131c35f00013d/)

