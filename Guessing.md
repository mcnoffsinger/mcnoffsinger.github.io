# Flowchart of Number Guessing Game
``` mermaid
flowchart TD
start((Start))
num[RNG 1-10]
while[while loop]
User[/User Input/]
range{In range?}
uNum[\Guessed Number/]
gNum[\Real Number/]
dome((End))
if1{=}
if2{greater than}
smol[\too small\]
beeg[\too large\]

num --> while 
subgraph while loop
    while -->User --> uNum 
    uNum --> range --yes--> if1
    if1 --no --> if2 --no --> smol --> while
    if2 --yes--> beeg --> while
    
    end
subgraph Startup
    start --> num
    end 
num --> gNum
gNum --> if1
gNum --> if2

range --no --> while

if1 --yes --> dome

style start fill:green,stroke-width:5, stroke: gold
style dome fill:lightblue ,stroke-width:5, stroke: white


```
## Documentation
In the startup phase, the Random number is chosen, then in the while loop the number is guessed until a. the number is in range, and b. the number is equal to the generated number. If the number is not equal to the RNG number, than a greater than operator will decide if the system returns "too small" or "too large."