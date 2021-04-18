### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[ModuleConstraint](./BrewedInk-WFC-ModuleConstraint.md 'BrewedInk.WFC.ModuleConstraint')
## ModuleConstraint.ShouldRemoveModule(BrewedInk.WFC.SlotEdge, BrewedInk.WFC.GenerationSpace, BrewedInk.WFC.Module, BrewedInk.WFC.ModuleSet) Method
The only required method of a WFC constraint.  
Given some edge and some module-in-question, should the module-in-question be removed from the edge's source's possibility space?  
  
When the WFC algorithm propagates information, every possible module per slot is checked against every neighboring slot. If ANY neighboring slot has a constraint that disqualifies the module-in-question, the module will be removed from the source's superposition. This in turn, causes a new propagation wave.  
```csharp
public abstract bool ShouldRemoveModule(BrewedInk.WFC.SlotEdge edge, BrewedInk.WFC.GenerationSpace space, BrewedInk.WFC.Module module, BrewedInk.WFC.ModuleSet modulesToRemove);
```
#### Parameters
<a name='BrewedInk-WFC-ModuleConstraint-ShouldRemoveModule(BrewedInk-WFC-SlotEdge_BrewedInk-WFC-GenerationSpace_BrewedInk-WFC-Module_BrewedInk-WFC-ModuleSet)-edge'></a>
`edge` [SlotEdge](./BrewedInk-WFC-SlotEdge.md 'BrewedInk.WFC.SlotEdge')  
The edge whose source slot's superposition is being checked. If the method returns true, the given module will be removed from the edge's source's slot's superposition.  
  
<a name='BrewedInk-WFC-ModuleConstraint-ShouldRemoveModule(BrewedInk-WFC-SlotEdge_BrewedInk-WFC-GenerationSpace_BrewedInk-WFC-Module_BrewedInk-WFC-ModuleSet)-space'></a>
`space` [GenerationSpace](./BrewedInk-WFC-GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')  
The generation space that this edge and module are apart of. The space is made available so that checks can be made for other available modules at the edge source and destination slots.  
  
<a name='BrewedInk-WFC-ModuleConstraint-ShouldRemoveModule(BrewedInk-WFC-SlotEdge_BrewedInk-WFC-GenerationSpace_BrewedInk-WFC-Module_BrewedInk-WFC-ModuleSet)-module'></a>
`module` [Module](./BrewedInk-WFC-Module.md 'BrewedInk.WFC.Module')  
The module-in-question. Should this module be removed from the edge source, because of the edge destination?  
  
<a name='BrewedInk-WFC-ModuleConstraint-ShouldRemoveModule(BrewedInk-WFC-SlotEdge_BrewedInk-WFC-GenerationSpace_BrewedInk-WFC-Module_BrewedInk-WFC-ModuleSet)-modulesToRemove'></a>
`modulesToRemove` [ModuleSet](./BrewedInk-WFC-ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
An advanced capability. Anything in this set will be removed from the edge source's superposition. You can manually add to the set, but only if you are extremely confident.  
  
#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
  
