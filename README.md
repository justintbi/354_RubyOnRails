# **Ruby On Rails**

## *Why did I choose to research Ruby on Rails?*
* Ruby has always been a programming language that I had heard about but did not have much experience in so I wanted to learn more about.
* I thought that it would be interesting to focus more on a framework for a language rather than an actual new language.
* I am interested in building websites and Ruby on Rails seemed like an interesting introduction to learning more about the process.

## *A Brief History of Ruby on Rails*
* Ruby on Rails was created in the year 2004 by a man named David Heinemeier Hansson in order to aid in the development process for another project that he was working on. 
* In 2005, Hansson released his project as open source and received the “Hacker of the Year” award from Google and O’Reilly. 
* Ruby on Rails has come a long way since then (363 versions since July 25, 2009) and is now in Version 6.0 with plenty of users.     

## *What kinds of tasks is Ruby on Rails particularly suitable for?*
The main tasks that Ruby on Rails is suited for is the development of website applications. Ruby on Rails was built for this main purpose and it excels at its job.
    (See 'Some Getting Started Steps' Below)
    
## *What are some examples of where Ruby on Rails is used successfully?*
* Github
* Twitch
* SoundCloud
* Kickstarter
* Hulu
* Square
* Urban Dictionary

## *Why should one consider Ruby on Rails for website development?*
* One of the main features that is intriguing about Ruby on Rails is that it is open source, meaning there is no licensing costs and that anybody can work on improving it. 
* There  is a clear desire in programmers’ minds to make Ruby on Rails have a sense of “convention over configuration”.
  * Convention over configuration is one of the principles that shapes the way Ruby on Rails operates by making it so developers do not have to deal with the unimportant minutiae of coding. 
  * Website developers using Ruby on Rails only have to deal with the overhead while behind the scenes actions are taking place.

## *Some features I found particularly interesting:*
* As a framework, Ruby on Rails serves as a collection of codes and tools that gives its users a mostly self documenting structure to organize their code. 
  * This structure helps to keep code organized and maintain a standard that is  sure to increase efficiency. 
* Ruby on Rails is fundamentally a framework for building web applications that uses the Ruby programming language as its base.
  * Many people who prefer coding in Ruby would find Ruby on Rails to be the best choice for website development.
* There is a vast collection of open source code available to use by any user.
  * Available open source code also allows for more efficiency and better management of one’s time.



### *Some Getting Started Steps (A Guide for Saying 'Hello Word' with Ruby on Rails:*
After downloading the necessary Ruby on Rails downloads:
Create a new application called hello world.  
`rails new hello_world`

In this directory, start a web server by lauching WEBrick:  
`rails server`

Can know navigate to http://localhost:3000 to view the server.

To get "Hello World" from Rails, we need to create at minimum a controller and a view.

1. A controller is needed to receive requests for the application.
1. Routing decides which controller receives which requests. Often, there is more than one route to each controller, and different routes can be served by different actions.
1. Each action's purpose is to collect information to provide it to a view.
1. A view's purpose is to display this information in a readable format.
1. An important distinction to make is that it is the controller, not the view, where information is collected. The view should just display that information.
1. By default, view templates are written in a language called ERB (Embedded Ruby) which is converted by the request cycle in Rails before being sent to the user.

To create a new controller, we need to run the controller generator and  
tell it we want a controller called welcome with an action called index:  
`rails generate controller welcome index`

Open the app/views/welcome/index.html.erb file in your text editor.  
Delete all of the existing code in the file, and replace it with the following single line of code:  
`<h1>Hello World from Rails!</h1>`

Now the controller and the view are set.
Next step is to tell Ruby on Rails when to show the Hello World message and where to find it.

Open the file config/routes.rb and uncomment the line:
`root "welcome#index"`

Now when navigating to http://localhost:3000 we can see the message "Hello World from Rails" in the browser.

# Sources
* https://www.bogotobogo.com/RubyOnRails/RubyOnRails_HelloWorld_Rails.php
* https://www.quora.com/What-makes-Rails-a-framework-worth-learning-in-2017/answer/David-Heinemeier-Hansson?utm_source=Syndicode%20blog&utm_medium=blogpost&utm_campaign=Syndicode%20news&utm_term=Ruby%20for%20beginners
* https://www.codingdojo.com/blog/ruby-on-rails-examples
* https://guides.rubyonrails.org/v3.2.13/getting_started.html#getting-up-and-running-quickly-with-scaffolding
* https://rubygems.org/gems/rails/versions
* https://www.rubyguides.com/2018/10/what-is-ruby-on-rails/
* https://www.rubyguides.com/ruby-tutorial/
* https://learn.onemonth.com/20-website-examples-built-with-ruby-on-rails/
