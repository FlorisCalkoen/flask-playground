

## Heroku & Git integration
First download and install Heroku [toolbelt](https://devcenter.heroku.com/articles/heroku-cli)

Create a Heroku application (stage and prod)  
```heroku create flask-playground-pro```  
```heroku create flask-playground-stage```

Add stage/prod branches to remote  
```git remote add stage git@heroku.com:flask-playground-stage.git```  
```git remote add pro git@heroku.com:flask-playground-pro.git``` 

Add heroku app as git remote  
```git:remote -a flask-playground-pro```  
```git:remote -a flask-playground-stage```

Now you can push  
```git push stage master```  
```git push pro master```