# sunshire-price

## To Start ##
*   npm install
*   node bin/www

## How To Use ##
*   HTTP POST

<code>
request.post(
              'https://root/price',
              {
              from_location: '3629 Lynoak Dr.',
              to_location: 'LAX TERMINAL 5',
              pickup_time: '2018-01-09 12:22:30'
              },
              function (error, response, body) {
                  //console.log('SEARCH FLIGHT SENDING PACKAGE');
                  //console.log(response);
                  if (!error && response.statusCode === 200) {
                      console.log(body);
                  } else {
                       console.log(error);
                  }
              }
          );
</code>