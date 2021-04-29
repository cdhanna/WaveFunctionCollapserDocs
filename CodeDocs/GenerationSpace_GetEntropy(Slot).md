#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.GetEntropy(Slot) Method
Calculates the current entropy of a slot.  
Entropy is roughly equal to the number of modules left in the slot's wave function. The contribution of each module is weighted by the module's weight. [Weight](Module_Weight.md 'BrewedInk.WFC.Module.Weight')  
The exact entropy calculation is ```csharp
 -sum( p log(p) ) ```
 over all modules where each p is the probability of the module.   
```csharp
public float GetEntropy(BrewedInk.WFC.Slot slot);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_GetEntropy(BrewedInk_WFC_Slot)_slot'></a>
`slot` [Slot](Slot.md 'BrewedInk.WFC.Slot')  
The slot to find the entropy of
  
#### Returns
[System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single')  
The current entropy of the slot
