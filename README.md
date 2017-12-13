
## Get ready to deploy your static website on Heroku.

It provides you quick guidance to host your site on Heroku with some minor changes and addition of new files in your project folder.

##### As you are aware that Heroku doesnt allow you to host static content, in order to do so you have to show case that your website runs on php than being static. Here are the steps that you have to follow:



- Go to root directory of your project where you have all your assets, CSS, JS etc. 
- Make sure that your root directory contains index.html(starting page) page, rename it to home.html.
- Add new file composer.json to root directory, open this file and type `{}` and save it.
- Add another file index.php to root directory, open this file and type `<?php include_once("home.html"); ?>` and save it.
- Open https://www.heroku.com/ login into your account or create one if you dont have it.
- Once you logged in, you can see new button in your dashboard on right top side of screen.
- Click on new -> create new app and provide name of your choice. Note: your link would be `https://{name of the app}.herokuapp.com/` 
- Install the Heroku CLI: https://devcenter.heroku.com/articles/heroku-cli
- Once you have installed Heroku CLI open your gitbash command window and type `$ heroku login` enter your heroku email and password.
- Navigate to your project folder by `$ cd my-project/` and type
    `$ git init                                                     `
    `$ heroku git:remote -a {name of the app}`
- Type following commands
`$ git add .`
`$ git commit -am "deploying my-app"`
`$ git push heroku master`

