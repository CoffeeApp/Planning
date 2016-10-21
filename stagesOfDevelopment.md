Stages of Development
===

### MVP

Establish sockets connections to allow us to send data from customer to shop.

### Phase 1 Objective - send one coffee order from customer to shop via api database

Data for phase 1 to be sent and received in the following structure.
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

### Customer-side

Coffee type: Flat white / Long Black / Latte

Milk: Full Milk (default) / Trim Milk / Soy Milk

Sugar: 0 sugar (default) / 1 sugar / 2 sugar / 3 sugar

Need name and phone number (must provide both) and have a datestamp for time order was placed.

### Business-side

Display:

For each coffee

* coffee type
* milk (only if not full milk)
* sugar (if not 0)

For each order

* time order placed
* name
* phone
* price

### API Database

Prepare to receive, send and store coffee orders in the following data structure.

```js
"order": {
  "shop": "Fidel's Cafe",
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
