#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.GetSlotOptions(Slot) Method
At any given moment, a slot may have many possible modules available to it. This method will give you the set of possible modules available on a slot.  
```csharp
public BrewedInk.WFC.ModuleSet GetSlotOptions(BrewedInk.WFC.Slot slot);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_GetSlotOptions(BrewedInk_WFC_Slot)_slot'></a>
`slot` [Slot](Slot.md 'BrewedInk.WFC.Slot')  
The slot whose available modules will be returned
  
#### Returns
[ModuleSet](ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
A set of modules representing all possible modules for the given slot
