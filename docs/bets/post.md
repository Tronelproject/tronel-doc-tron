/bets POST
=========

check all new bets, and send new bets.

* route: `/bets`
* method: `POST`
* url query: none
* body: none

* response: `[Object]`

  * sample response
    ```javascript
    [
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
    ]
    ```
