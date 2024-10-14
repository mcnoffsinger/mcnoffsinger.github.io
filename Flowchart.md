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


start --> num --> while -->User --> uNum
num --> gNum
gNum --> if1
uNum --> range --yes--> if1
range --no --> while
if1 --no --> while
if1 --yes --> dome

```