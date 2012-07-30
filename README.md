flashcardio
============

How to get flashcardio running on your local machine and how to deploy it
on Heroku.

Development on your local machine
---------------------------------

Be sure to have Git, Java and Maven installed. Additionally you need the
heroku toolbelt from `https://toolbelt.heroku.com/`
Clone the project from
`git@github.com:stefanbirkner/flashcardio.git`
and run the server with

    mvn package
    sh target/bin/webapp

Continuous Integration
----------------------

There's a Jenkins server on CloudBees:
`https://stefanbirkner.ci.cloudbees.com/`

Deploy flashcardio on Heroku
----------------------------

Create a remote branch on Heroku

    heroku create

Add it as remote

    git remote add heroku git@heroku.com:flashcardio.git

and deploy flashcardio by pushing it to Heroku

    git push heroku master
