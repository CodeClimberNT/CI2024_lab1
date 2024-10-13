# Laboratory 1

## Customization

I modified the fitness function such as it will consider:

1. If a solution is valid
2. Prefer fewer number of sets that cover the same element (**redundancy reduction**)

## Results

| Instance | UNIVERSE_SIZE | NUM_SETS | DENSITY | Fitness                    | Cost         | Valid Solution |
| -------- | ------------- | -------- | ------- | -------------------------- | ------------ | -------------- |
| 1        | 100           | 10       | 0.2     | -28916.55                  | 278.02       | True           |
| 2        | 1_000         | 100      | 0.2     | -955215946.71              | 20642.61     | True           |
| 3        | 10_000        | 1_000    | 0.2     | -533024922555469.88        | 2305573.47   | True           |
| 4        | 100_000       | 10_000   | 0.1     | -15364790913551548416.00   | 124566203.87 | True           |
| 5        | 100_000        | 10_000    | 0.2     | -600066144764060762112.00  | 268547654.43 | True           |
| 6        | 100_000        | 10_000    | 0.3     | -5303792096180067893248.00 | 423510822.08 | True           |


### Note
Actually the column *Valid Solution* was not needed as the fitness would be `-inf` if that was `false`, but for better documentation I decided to leave it as well.


## Contribution
Most of the heavy lifting was done thanks to [ChatGPT](https://chatgpt.com/) (but as an AI artist may say: *but i made the prompt that generate this result :p*). 

As usual something wasn't right or wasn't optimized as I intended to so I made a lot of fine tuning to achieve my idea.

I use the philosophy proposed by the professor to use 
a *tweak*/*mutate* function to hill climb or an *evaluate*/*fitness* to have a metric for the height in the landscape of the problem.