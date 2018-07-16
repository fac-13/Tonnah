# Gif, Set, Match (aka Tonnah)
https://gif-set-match.herokuapp.com/

### Description: 
_**See a Gif, Find a Gif!**_

Gif Set Match is a gif finding game, where users will see a gif and then have a limited amount of time to find that gif among other gifs. 

Gif Set Match was made using React and the [Giphy API](https://developers.giphy.com/).

Gif Set Match is hosted on Heroku, click [here](https://gif-set-match.herokuapp.com/) to play!

The game was built over 2 days to learn react. 

---

### User Stories 
- [x] Users will see a random Gif from the Giphy Api which they will have to find (the specified gif)
- [x] Users will have to find the specified gif among other gifs 
- [x] Users will have a limited amount of time to find the specified gif 
- [x] Users will be able to see their score 
- [x] The game will continue until the user loses (i.e. they fail to find the gif in time)
- [ ] Users can enter their name at the start of the game 

_**Stretch Goal**_
- [ ] Users can see where they rank on a scoreboard


---
### File Structure

```
Gif Set Match
├── Client
│       ├── __mocks__
|       |   ├── fileMock.js
│       │   └── styleMock.js
│       ├── public
|       |   ├── index.html
│       │   └── style.css
|      ├── Src
|       │  ├── Components
|       │       ├── board
|       |       |   ├── gameover
|       |       |   |    ├── gameover.js
|       |       |   |    └── styles.css
|       |       |   ├── photogroup
|       |       |   |    ├── photogroup.js
|       |       |   |    └── styles.css
|       |       |   ├── singlephoto
|       |       |   |    ├── singlephoto.js
|       |       |   |    └── styles.css
|       |       |   ├── timer
|       |       |   |    └──  timer.js
|       |       |   ├── board.js
|       |       |   ├── board.test.js
|       |       |   ├── dummyresponse.js
|       │       │   └── styles.css
|       │       ├── App.js
|       │  ├── Utils
|       │       └── datahelpers.js
|       │  ├── index.js
├── server/src
|       ├── index.js
├── .babelrc
├── .eslintrc
├── .gitignore
├── README.md
├── package-lock.json
├── package.json

```

---
### Tech Stack and Tools
The project uses: 

| Front End         | Back End       | Testing       | Tools   |
| -------------     | -------------  |:-------------:| -----:  |
| React             | Node           | Jest          | Netlify |
| JSX               | Express        |               | Parcel  |
| Javascript(ES6)   |                |               | Babel   |
| HTML5             |                |               | Eslint  |
| CSS3              |                |               |         |

___

### If we had more time we would...
- [ ] Fix the rendering issue where the specified gif loads before all other gifs on the first round
- [ ] Allow users to enter their username 
- [ ] Create a scoreboard feature 
- [ ] write more tests 

### Challenges 
- Working out where to keep state
- Trying to fix the delay on the initial render
    - On the page where the user must find the specified gif among the other gifs, the specified gif initially loads first so its easy to find. 
    - This effect only happens the first time the user plays 
    - We haven't managed to fix this yet  
