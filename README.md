# Event Packing 90 Min Takehome
> Tester: Eli
> date: 3/19/2020

## Setup 
This project depends on `python-3.7` and `pipenv` install those first

Add test dependencies 
```
pipenv shell
```

Run tests (normally we would separate those out but for the sake of convenience I kept them in the same file)
```
pytest event_packing.py
```

## Approach
I wanted to make sure I came up with a computationally efficient solution first. I chose to order the meetings in descending order figuring the big meetings would cause the most merge conflicts anyways and then we could fill in around them with the remaining smaller meetings. 


Given more time and depending on the speed requirements the next approach I would try would be to run a few permutations of that solution in which we shuffle the order of the meetings with the same length in meetings_desc. This might give us a few incremental wins with minimal cost.
