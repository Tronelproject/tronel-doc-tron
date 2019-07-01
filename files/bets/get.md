/bets GET
=========

list of all bets.

* route: `/bets`
* method: `GET`
* url query: none
* body: none

* response: `[Object]`

  * sample response:
    ```javascript
    [
      {
        id: '5ceb99b92e98592cd9940d53',
        address: 'TVWmQKmaJNowQewdGz16ekW2jQgXwaAfCc',
        creator: 'TAzaDwcKucTz9YJwMWotXKib4iH4RYG8PJ',
        acceptor: 'T9yD14Nj9j7xAB4dbGeiX9h8unkKHxuWwb',
        currency: 'bitcoin',
        predictPrice: 8000,
        predictTime: 1559212920, // based on seconds not miliseconds
        predictType: 1,
        submittedPrice: 0,
        disabled: false,
        done: false,
        betAmount: 10 // 10 in sun
      }
    ]
    ```
