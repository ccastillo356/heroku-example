# heroku-example

Pre-steps:

1. Make sure you have `const PORT = process.env.PORT || 3000;` in your `server.js`.
2. Make sure you have `"start": "node server.js"` in your `package.json` under your `"scripts"` section.

Heroku steps:

1. First do `heroku login`.
2. Login to your heroku account when the browser opens.
3. Return to the terminal.

4. Do `heroku create`. This creates an app in your heroku account for you.
   (If you do `git remote -v` at this point, you'll be able to see a Heroku remote in addition to the one for github.com.)
5. Do `git init` to reinitialize a git repository in your heroku app.
6. `git add .` and `git commit -m "deploying app"`
7. `git push heroku master` (and you can push to github as well with the normal `git push origin master`)
8. `heroku open` to see your deployed app (can also be done from `settings` tab in heroku.com)
