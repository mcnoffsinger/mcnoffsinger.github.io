# Flowchart of Number Guessing Game
``` mermaid
flowchart TD
start((Start))
num[RNG 1-10]
while(while loop)
User[/User Input/]
range{In range?}
uNum[\Guessed Number/]
gNum[\Real Number/]
dome((End))
if1{=}


num --> while 
subgraph while loop
    while -->User --> uNum 
    uNum --> range --yes--> if1
    end
subgraph Startup
    start --> num
    end 
num --> gNum
gNum --> if1

range --no --> while
if1 --no --> while
if1 --yes --> dome


style start fill:green,stroke-width:5, stroke: gold
style dome fill:blue ,stroke-width:5, stroke: white
style uNum fill:darkblue
style gNum fill:darkblue

```