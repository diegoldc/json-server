# 1up

This repository is a [json-server](https://github.com/diegoldc/json-server) created to feed data into the React Application below.

#### [Client Repo here](https://github.com/diegoldc/1up-webapp)

# Server Structure

## Collections

### reviews

```javascript
{
  rating,
    content,
    gameId,
    userName,
    profilePic,
    id,
    wouldRecommend,
    profileId,
    gameName;
}
```

### myGames

```javascript
{
  name,
  cover,
  gameId,
  platform,
  isGameCompleted,
  screenshots,
  hoursPlayed,
  id;
}
```

### profiles

```javascript
{
  id, 
  user, 
  profilePic, 
  storeCredit;
}
```

## Used API Endpoints in the App

| HTTP Method | URL                  | Request Body                                                                             | Description                        |
| ----------- | -------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------- |
| GET         | `/reviews`           |                                                                                          | Sends all reviews                  |
| GET         | `/reviews/?gameId`   |                                                                                          | Sends all reviews of selected game |
| GET         | `/reviews/?profileId`|                                                                                          | Sends all reviews made by user     |
| GET         | `/reviews/:reviewId` |                                                                                          | Sends selected review              |
| POST        | `/reviews`           | {rating, content, gameId, userName, profilePic, id, wouldRecommend, profileId, gameName} | Creates a new review               |
| PATCH       | `/reviews/:reviewId` | {rating, content}                                                                        | Edits a review object              |
| DELETE      | `/reviews/:reviewId` |                                                                                          | Deletes a review object            |
| GET         | `/myGames`           |                                                                                          | Sends all myGames                  |
| GET         | `/myGames/:gameId`   |                                                                                          | Sends selected game                |
| POST        | `/myGames`           | {name, cover, gameId, platform, isGameCompleted, screenshots, hoursPlayed, id}           | Creates a new myGame               |
| PUT         | `/myGames/:myGameId` | {name, cover, gameId, platform, isGameCompleted, screenshots, hoursPlayed, id}           | Edits data from myGame             |
| PATCH       | `/myGames/:myGameId` | {screenshots}                                                                            | Adds screenshots to myGame         |
| DELETE      | `/myGames/:myGameId` |                                                                                          | Deletes a myGame object            |
| GET         | `/profile`           |                                                                                          | Sends profile                      |



## Links

### Collaborators

[Developer 1 name](https://github.com/TanoPalazzo14)

[Developer 2 name](https://github.com/diegoldc)

### Project

[Repository Link Client](https://github.com/diegoldc/1up-webapp)

[Repository Link Server](https://github.com/diegoldc/json-server)

[Deploy Link](https://1up-app.netlify.app/)


### Slides

[Slides Link](https://docs.google.com/presentation/d/1mkqT8JrSzoPOuVwp_JhfJF-_TxbVadvvHDhwdmpvHWE/edit?usp=sharing)
