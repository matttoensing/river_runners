# River Runners
- One of my favorite places to hang out in the summer!
- Fork and clone this repo
- Complete the interaction patterns for Iteration 1 and 2
- No interaction patterns for Iteration 3

## Iteration 1

```
[1] pry(main)> require './lib/passenger'
=> true
[2] pry(main)> billy = Passenger.new({first_name: 'Billy', last_name: "Lowell", age: 28, max_tip_amount: 50, excitement_level: 6})
=> #<Passenger:0x00007fc587298d18
[3] pry(main)> billy.full_name
=> "Billy Lowell"
[4] pry(main)> billy.age
=> 28
[5] pry(main)> billy.max_tip_amount
=> 50
[6] pry(main)> billy.excitement_level
=> 6
```

## Iteration 2

```
[1] pry(main)> require './lib/passenger'
=> true
[2] pry(main)> require './lib/guide'
=> true
[3] pry(main)> billy = Passenger.new({first_name: 'Billy', last_name: "Lowell", age: 28, max_tip_amount: 50, excitement_level: 6})
=> #<Passenger:0x00007f9800295758
[4] pry(main)> johanna = Passenger.new({first_name: 'Johanna', last_name: "Smith", age: 22, max_tip_amount: 35, excitement_level: 8})
=> #<Passenger:0x00007f9800237a40
[5] pry(main)> phil = Guide.new("Phil", "Pandora", [billy, johanna])
=> #<Guide:0x00007f980018ccd0
[6] pry(main)> phil.name
=> "Phil"
[7] pry(main)> phil.boat_name
=> "Pandora"
[8] pry(main)> phil.passengers
=> [#<Passenger:0x00007f9800295758,
 #<Passenger:0x00007f9800237a40]
[9] pry(main)> phil.boat_flipped?
=> false
[10] pry(main)> phil.passengers_excitement
=> {"Billy Lowell"=>6, "Johanna Smith"=>8}
[11] pry(main)> phil.tips_made
=> 0
[12] pry(main)> phil.trip_over
[14] pry(main)> phil.tips_made
=> 85
[15] pry(main)> phil.boat_flipped = true
=> true
[16] pry(main)> phil.trip_over
[17] pry(main)> phil.tips_made
=> 42.5
```

## Iteration 3
Your task is to create a way for each guide service to track each guides tips at the end of each day for tax purposes. The guide service has multiple guides and each guide has more than one customer that may or may not tip the guide at the end of the trip.

  - The guide service has a unique name and a way to read that data
  - The guide service has multiple guides and a way to keep track of that data
  - The guide service can keep track of each guide and accompanying passengers
  - The guide service can record each guides tips at the end of each trip

Use iteration 1 and 2 to help accomplish your task. 
