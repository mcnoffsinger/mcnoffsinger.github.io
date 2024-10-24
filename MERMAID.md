# Mermaid diagram
## Humanities 110 notes doc evolution
### Suggested by Christopher
```mermaid
flowchart TD
begin((humanities begins)) 
oppenheim(someone creates doc bomb)
boom{{someone activates doc bomb}}
revert[revert the doc]
gif(someone adds gif to the notes)
shrink(gif is shrunk)
del(gif is deleted)
commie[[someone manifesto bombs the doc]]
defuse(someone defuses the bomb)
notes((we actually start taking notes))
ban(we ban someone)
revenge{{banned ruins the doc}}

good(we take good notes)
bad{{we take bad notes}}
pass{we pass the test}

begin--> oppenheim --> defuse --> notes
begin --> commie
boom --> revert
revert --nice--> begin
bad --> revert
boom --> ban --> revenge --> revert
subgraph The Note-Taking Zone
    notes --> gif --good-->shrink
    gif --bad-->del --> gif
    
    notes --> good --> pass
    notes --> bad 
    end
subgraph The Bomb Zone
    oppenheim--> boom
    commie --> boom
    end

style boom fill:red,stroke:black,stroke-width:10
style revenge fill:red,stroke:black,stroke-width:10
style bad fill:red,stroke:black,stroke-width:10
style pass fill:green,stroke:gold,stroke-width:10
```



