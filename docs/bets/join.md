/bets/:id/join PUT
=========

call this route when another user joined the bet.

* route: `/bets/:id/join`
  * id: bet id.
* method: `PUT`
* url query: none
* body: none

* response: `Object`

  * sample response
    ```javascript
    {
      id: '5ceb99b92e98592cd9940d53',
      address: '0x0000000000000000000000000000000000000000',
      creator: '0x0000000000000000000000000000000000000000',
      joiner: '0x0000000000000000000000000000000000000000',
      currency: 'bitcoin',
      predictPrice: 8000,
      predictTime: 1559212920, // based on seconds not miliseconds
      predictType: 1,
      submittedPrice: 0,
      disabled: false,
      done: false,
      balance: 10 // 10 TPI
    }
    ```

* error:
  * status: `400`
  * reason: bet id is not found.
  * response:
  ```javascript
  {
    status: 400,
    error: {
      // error object
    }
  }
  ```
