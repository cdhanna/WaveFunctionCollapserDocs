#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## ModuleConstraint Class
The base type for all WFC constraints. Feel free to subclass this type and make your own constraints.   
```csharp
public abstract class ModuleConstraint
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ModuleConstraint  

Derived  
&#8627; [AdjacencyConstraint](AdjacencyConstraint.md 'BrewedInk.WFC.AdjacencyConstraint')  
### Methods

***
[ShouldRemoveModule(SlotEdge, GenerationSpace, Module, ModuleSet)](ModuleConstraint_ShouldRemoveModule(SlotEdge_GenerationSpace_Module_ModuleSet).md 'BrewedInk.WFC.ModuleConstraint.ShouldRemoveModule(BrewedInk.WFC.SlotEdge, BrewedInk.WFC.GenerationSpace, BrewedInk.WFC.Module, BrewedInk.WFC.ModuleSet)')

The only required method of a WFC constraint.  
Given some edge and some module-in-question, should the module-in-question be removed from the edge's source's possibility space?  
  
When the WFC algorithm propagates information, every possible module per slot is checked against every neighboring slot. If ANY neighboring slot has a constraint that disqualifies the module-in-question, the module will be removed from the source's superposition. This in turn, causes a new propagation wave.  
