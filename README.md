# Adventures of Jojo and Junior

### Todo
- [ ] Backend
  - [ ] swagger
    - [ ] post create user
    - [ ] post login
    - [ ] post create game
    - [ ] get open/running games
    - [ ] get statistics
      - [ ] user stats
      - [ ] global stats?
      - [ ] time played
      - [ ] characters played/how many times
      - [ ] enemies bonked
        - [ ] by type
      - [ ] unique other players played with
  - [ ] express server
  - [ ] route middleware
    - [ ] post create user
    - [ ] post login
    - [ ] post create game
    - [ ] get open/running games
    - [ ] get statistics
      - [ ] user stats
      - [ ] global stats?
      - [ ] time played
      - [ ] characters played/how many times
      - [ ] enemies bonked
        - [ ] by type
      - [ ] unique other players played with
  - [ ] socket stuff
    - [ ] wss?
    - [ ] only connect with auth token after logged
    - [ ] events
      - [ ] client
        - [ ] move (left, right, up, down)
        - [ ] attack
        - [ ] jump? extension
      - [ ] server - calculates state i.e. if something got hit
        QUESTION - one event, i.e. 'new state' that has all info
          {
            playerData: [
              {
                id: 1,
                positionX: 10,
                positionY: 10,
                facing: right,
                health: 5
              }
            ],
            enemyData: [
              {
                id: 5,
                positionX: 15,
                positionY: 15,
                facing: left,
                health: 1
              }
            ]
          }
        OR multiple events
        player new position =
        {
          id: 1,
          positionX: 11,
          positionY: 11,
          facing: right
        }
        player new health:
        {
          id: 1,
          health: 3
        }
        enemy new health:
        {
          id: 5,
          health: 0
        }
- [ ] Frontend
  - [ ] login, create user page
  - [ ] create, join game page
  - [ ] stats
  - [ ] game