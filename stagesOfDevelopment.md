Stages of Development
===

### MVP

~~Establish sockets connections to allow customer and shop to send data to each other.

___

### Release 1

Target Deadline - E.O.D Saturday

#### customer side to be able to send one full coffee order (including multiple coffees with different specs) to single shop via api database: Details to include:

For each coffee

* coffee type
* milk (only if not full milk)
* sugar (if not 0)

For each order

* time order placed
* name
* phone
* price

#### shop side to be able to receive and display one full coffee order (including multiple coffees with different specs) from a single user via api database: Details to include:

Data object to be sent and received in the following structure.
```js
"order": {
  "name": "Jonathan",
  "phone": "021 098 2763",
  "comment": "no sugar"
}
```
```js
"order": {
  "order_id": 1,
  "shop_id": 234,
  "coffees": [
    {
      "type": "flat white",
      "qty": 1,
      "milk": "trim",
      "sugar": 1
    },
    {
      "type": "americano",
      "qty": 2,
      "milk": "soy",
      "sugar": 0
    }  
  ],
  "details": {
    "price": 6.00,
    "name": "Jeremy",
    "phone": "021 225 555",
    "ordered": "Fri Oct 21 2016 10:39:50 GMT+1300 (NZDT)"
  }
}
```

* shop-side to be able update order status and start countdown timer when start making coffee order.

* customer-side to be able see countdown timer when shop-side updates order status.
___

### Release 2

Target Deadline - EOD Sunday

User can prepare coffee order and view prices, distance and user rating for a minimum of 5 nearby shops inlcuding:

* Southern Cross
* Laundry
* Fidel's Cafe
* Emporio Coffee
* Raglan roast 

User can select one of the available coffee shops to order from and send order to that particular user at business end.

Have some form of google maps api working in the app.

___

### Release ? ideas

Target Deadline - EOD Tuesday

Customers can filter nearby shops by price, distance & rating. User can also get directions from google maps api to chosen business.

Customer can edit and cancel order if coffee order is not yet being made.

Customer can submit feedback/ rating on their coffee order after consumption.

AI element in voice activation, mini game etc.

More ideas please......

## ALL SUBTEAMS AIM TO BE FINISHED BACKLOG BY E.O.D TUESDAY. This leaves all day Wednesday for all teams to:

* help other teams that may not have hit this deadline.
* user testing
* debugging
* refactor code so it looks as delicious as possible.
* Polish css / logo design / UI / UX
* Fully understand how the entire app works.
* Business feedback/ endorsements we can use on pitch day.
