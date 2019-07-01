/bets/:id/join PUT
=========

when other user joined to bet.

* route: `/bets/:id/join`
* id: bet id.
* method: `PUT`
* url query: none
* body: none

* response: `Object`
  * sample response:
    ```javascript
    {
      id: '5ceb99b92e98592cd9940d53',
      address: 'TVWmQKmaJNowQewdGz16ekW2jQgXwaAfCc',
      creator: 'TAzaDwcKucTz9YJwMWotXKib4iH4RYG8PJ',
      acceptor: 'TDyWa7saV4hpZUup45arrQjoRoe13Wf5aY',
      currency: 'bitcoin',
      predictPrice: 8000, // in sun
      predictTime: 1559212920, // based on seconds not miliseconds
      predictType: 1,
      submittedPrice: 0,
      disabled: false,
      done: false,
      betAmount: 10 // 10 in sun
    }
    ```

  * error:
    * status: `400`
    * reason: bet id is not found or couldn't interact with smart contract.
    * response:
    ```javascript
    {
      status: 400,
      error: {
        // error object
      }
    }
    ```
