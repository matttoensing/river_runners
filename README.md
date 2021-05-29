# River Runners
- One of my favorite places to hang out in the summer!
- Fork and clone this repo
- Complete the interaction patterns for Iteration 1 and 2
- No interaction patterns for Iteration 3

## Iteration 1

```
pry(main)> require './lib/passenger'
=> true
pry(main)> billy = Passenger.new({first_name: 'Billy', last_name: "Lowell", age: 28, max_tip_amount: 50, excitement_level: 6})
=> #<Passenger:0x00007fc587298d18
pry(main)> billy.full_name
=> "Billy Lowell"
pry(main)> billy.age
=> 28
pry(main)> billy.max_tip_amount
=> 50
pry(main)> billy.excitement_level
=> 6
```

## Iteration 2

```
pry(main)> require './lib/passenger'
=> true
pry(main)> require './lib/guide'
=> true
pry(main)> billy = Passenger.new({first_name: 'Billy', last_name: "Lowell", age: 28, max_tip_amount: 50, excitement_level: 6})
=> #<Passenger:0x00007f9800295758
pry(main)> johanna = Passenger.new({first_name: 'Johanna', last_name: "Smith", age: 22, max_tip_amount: 35, excitement_level: 8})
=> #<Passenger:0x00007f9800237a40
pry(main)> phil = Guide.new("Phil", "Pandora", [billy, johanna])
=> #<Guide:0x00007f980018ccd0
pry(main)> phil.name
=> "Phil"
pry(main)> phil.boat_name
=> "Pandora"
pry(main)> phil.passengers
=> [#<Passenger:0x00007f9800295758,
 #<Passenger:0x00007f9800237a40]
pry(main)> phil.boat_flipped?
=> false
pry(main)> phil.passengers_excitement
=> {"Billy Lowell"=>6, "Johanna Smith"=>8}
pry(main)> phil.tips_made
=> 0
pry(main)> phil.trip_over
pry(main)> phil.tips_made
=> 85
pry(main)> phil.boat_flipped = true
=> true
pry(main)> phil.trip_over
pry(main)> phil.tips_made
=> 42.5
```

## Iteration 3
Your task is to create a way for each guide service to track each guides tips at the end of each day for tax purposes. The guide service has multiple guides and each guide has more than one customer that may or may not tip the guide at the end of the trip.

  - The guide service has a unique name and a way to read that data
  - The guide service has multiple guides and a way to keep track of that data
  - The guide service can keep track of each guide and accompanying passengers
  - The guide service can record each guides tips at the end of each trip

Use iteration 1 and 2 to help accomplish your task. 
