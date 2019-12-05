# **Ruby On Rails**

## *Why did I choose to research Ruby on Rails?*

## *A Brief History of Ruby on Rails*

## *What kinds of tasks is Ruby on Rails particularly suitable for?*

## *What are some examples of where Ruby on Rails is used successfully?*

## *Why should one consider Ruby on Rails for website development?*

## *Some features I found particularly interesting:*

#### *Some Getting Started Steps (A Guide for Saying 'Hello Word' with Ruby on Rails:*
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
