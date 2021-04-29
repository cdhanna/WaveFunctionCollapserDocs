#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[ModuleConstraint](ModuleConstraint.md 'BrewedInk.WFC.ModuleConstraint')
## ModuleConstraint.ShouldRemoveModule(SlotEdge, GenerationSpace, Module, ModuleSet) Method
The only required method of a WFC constraint.  
Given some edge and some module-in-question, should the module-in-question be removed from the edge's source's possibility space?  
  
When the WFC algorithm propagates information, every possible module per slot is checked against every neighboring slot. If ANY neighboring slot has a constraint that disqualifies the module-in-question, the module will be removed from the source's superposition. This in turn, causes a new propagation wave.  
```csharp
public abstract bool ShouldRemoveModule(BrewedInk.WFC.SlotEdge edge, BrewedInk.WFC.GenerationSpace space, BrewedInk.WFC.Module module, BrewedInk.WFC.ModuleSet modulesToRemove);
```
#### Parameters
<a name='BrewedInk_WFC_ModuleConstraint_ShouldRemoveModule(BrewedInk_WFC_SlotEdge_BrewedInk_WFC_GenerationSpace_BrewedInk_WFC_Module_BrewedInk_WFC_ModuleSet)_edge'></a>
`edge` [SlotEdge](SlotEdge.md 'BrewedInk.WFC.SlotEdge')  
The edge whose source slot's superposition is being checked. If the method returns true, the given module will be removed from the edge's source's slot's superposition.
  
<a name='BrewedInk_WFC_ModuleConstraint_ShouldRemoveModule(BrewedInk_WFC_SlotEdge_BrewedInk_WFC_GenerationSpace_BrewedInk_WFC_Module_BrewedInk_WFC_ModuleSet)_space'></a>
`space` [GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')  
The generation space that this edge and module are apart of. The space is made available so that checks can be made for other available modules at the edge source and destination slots. 
  
<a name='BrewedInk_WFC_ModuleConstraint_ShouldRemoveModule(BrewedInk_WFC_SlotEdge_BrewedInk_WFC_GenerationSpace_BrewedInk_WFC_Module_BrewedInk_WFC_ModuleSet)_module'></a>
`module` [Module](Module.md 'BrewedInk.WFC.Module')  
The module-in-question. Should this module be removed from the edge source, because of the edge destination?
  
<a name='BrewedInk_WFC_ModuleConstraint_ShouldRemoveModule(BrewedInk_WFC_SlotEdge_BrewedInk_WFC_GenerationSpace_BrewedInk_WFC_Module_BrewedInk_WFC_ModuleSet)_modulesToRemove'></a>
`modulesToRemove` [ModuleSet](ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
An advanced capability. Anything in this set will be removed from the edge source's superposition. You can manually add to the set, but only if you are extremely confident. 
  
#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
Return true if the module should be removed from the edge's source's super position, because the constraint is invalid. Return false if the module doesn't break the constraint.
