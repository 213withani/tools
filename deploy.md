
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
