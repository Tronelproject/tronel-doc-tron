/bets POST
=========

add a new bet to database and set jobs for setting price.

* route: `/bets`
* method: `POST`
* url query: none
* body: `JSON`

```json
{
  "address": "TVWmQKmaJNowQewdGz16ekW2jQgXwaAfCc"
}
```

* response: `Object`
  * sample response:
    ```javascript
    {
      id: '5ceb99b92e98592cd9940d53',
      address: 'TVWmQKmaJNowQewdGz16ekW2jQgXwaAfCc',
      creator: 'TAzaDwcKucTz9YJwMWotXKib4iH4RYG8PJ',
      acceptor: 'T9yD14Nj9j7xAB4dbGeiX9h8unkKHxuWwb', // default address, genesis address. it means nobody joined
      currency: 'bitcoin',
      predictPrice: 8000,
      predictTime: 1559212920, // based on seconds not miliseconds
      predictType: 1,
      submittedPrice: 0,
      disabled: false,
      done: false,
      betAmount: 10 // 10 sun
    }
    ```

  * error:
    * status: `400`
    * reason: contract address is invalid or contract is invalid.
    * response:
    ```javascript
    {
      status: 400,
      error: {
        // error object
      }
    }
    ```
