
# Deploy to github pages
https://medium.freecodecamp.org/surge-vs-github-pages-deploying-a-create-react-app-project-c0ecbf317089

# AWS 
https://www.airpair.com/aws/posts/building-a-scalable-web-app-on-amazon-web-services-p1

# Deploying a Node.js app to AWS Elastic Beanstalk
## A simple Hello World example using the EB CLI
https://medium.com/@xoor/deploying-a-node-js-app-to-aws-elastic-beanstalk-681fa88bac53

# Heroku

https://blog.heroku.com/deploying-react-with-zero-configuration

```
npm install -g create-react-app
create-react-app my-app
cd my-app
git init
heroku create -b https://github.com/mars/create-react-app-buildpack.git
git add .
git commit -m "react-create-app on Heroku"
git push heroku master
heroku open
```

# surge and GITHUB PAGES
https://medium.freecodecamp.org/surge-vs-github-pages-deploying-a-create-react-app-project-c0ecbf317089

https://hackernoon.com/how-to-create-and-deploy-a-create-react-app-with-recharts-the-wikiquotes-api-and-a-data-set-1f3a90fccb2d

1. Go to your package.json and add two new fields as so:
{
    ...
    "private": true, //below this add:
    "homepage": "https://github_username.github.io/repository_name",
    ... 
    "scripts": {
        "eject": "react-scripts-eject", //below this add:
        "deploy: "npm run build&&gh-pages -d build"
    ...
}
2. Then do this: npm install --save-dev gh-pages. Push your code to master.
3. npm run build which will create a bundle of all the code in your application (after running it, look in your file system and you will see a build folder containing all of the code in a tightly woven, unreadable format).
4. npm run deploy is the last step in the terminal
5. Go onto your GitHub account. Go to the applications page, then to settings, scroll down until you reach the GitHub Pages, click the Source dropdown and find gh-pages branch then wait a moment and you are…
Deployed!
