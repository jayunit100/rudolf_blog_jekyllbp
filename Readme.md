Official heroku server : http://blooming-meadow-7199.herokuapp.com/ :::: blooming-meadow-7199

Creating a Jekyll App with a Custom Jekyll Buildpack on Heroku Cedar (from GitHub)
===================
    gem install jekyll
    git clone git@github.com:markpundsack/jekyll-heroku.git
    cd jekyll-heroku
    jekyll --server --auto
    Open your browser and go to http://localhost:4000.

Deploying to Heroku
-------------------
    gem install heroku
    heroku create --stack cedar --buildpack http://github.com/markpundsack/heroku-buildpack-jekyll.git
    OR 
    heroku config:add BUILDPACK_URL=http://github.com/markpundsack/heroku-buildpack-jekyll.git
    git push heroku master
    
