# metacritic_bot

A simple, unofficial telegram bot which searches and returns movies, videogames and music albums info from metacritic.com.

## Features
1. Videogame data searcher.
2. Movie data searcher. *
3. TV series data searcher. *
4. Music album data searcher (needs some improvement).*
5. Suggestion searcher.

\* Previously available. Due to changes in the metacritic website interface since the first version of this bot (released in 2016), the bot can't fetch and return in most cases the data of movies, tv series and music albums. Nevertheless, the game and suggestion searcher are still fully functional.

I'll try to fix the issues with the movie, TV series and Music Album searcher some day.


## Commands
```
Usage mode:
/movie movie_name: Search for a movie data in metacritic 
/tv series_name/season season_number: Search for a TV series scores in metacritic
/game console_name/game_name: Search for a videogame data of an especific console in metacritic 
/music album/singer_or band: Search for a music album data of a singer or a band in metacritic 
/search [movie|tv|game|album]/[movie_name|series_name|game_name|album_name]: Searches and return a list of suggestions for a entered movie/tv series/game/album query 
```

## Screenshots

![example 7](botscreenshot7.png)
![example 1](botscreenshot1.png)
![example 2](botscreenshot2.png)
![example 3](botscreenshot3.png)
![example 4](botscreenshot4.png)
![example 5](botscreenshot5.png)
![example 6](botscreenshot6.png)

## Try it yourself

1. Create your own bot via [@BotFather](https://telegram.me/BotFather), make your own bot and get its token.
2. Copy and paste your token in bot.js file in 'YOUR TOKEN'
3. Create a heroku account and clone node's heroku tutorial project.
4. Replace those files with these, add and commit the changes. 
5. Make your first push to heroku master `git push heroku master`. Open the app in the command console with 'heroku open'
6. Get the address of your heroku web application in your web browser and paste it in bot.js file in 'YOUR WEBHOOK'
7. Add, commit the changes and push the project again
8. Enjoy!

##A little thing to consider
The bot might have some problems finding your wanted result if your query contains the name of a movie/game/series/album which name has been used in another
products or if it has remakes. In this case, you must specify the year of release after the name of what you want to search.

For example

The input '/movie frozen' will return the data from a thriller from 2010 and not the popular disney animation movie from 2013.

To get Disney's Frozen data, you must input '/movie frozen 2013'.

You can search the year of release of a movie, tv series, game or album using the '/search' function.

## References
Here I list some useful tutorials and similar projects which helped me to develop this bot:
- [Scraping the Web With Node.js](https://scotch.io/tutorials/scraping-the-web-with-node-js)
- [Build a telegram bot using node.js and heroku](http://mvalipour.github.io/node.js/2015/11/10/build-telegram-bot-nodejs-heroku/)
- [aabreuglez's wordReferenceBot] (https://github.com/aabreuglez/wordReferenceBot)

