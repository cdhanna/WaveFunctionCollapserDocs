### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[GenerationSpace](./BrewedInk-WFC-GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.GetSlotOptions(BrewedInk.WFC.Slot) Method
At any given moment, a slot may have many possible modules available to it. This method will give you the set of possible modules available on a slot.  
```csharp
public BrewedInk.WFC.ModuleSet GetSlotOptions(BrewedInk.WFC.Slot slot);
```
#### Parameters
<a name='BrewedInk-WFC-GenerationSpace-GetSlotOptions(BrewedInk-WFC-Slot)-slot'></a>
`slot` [Slot](./BrewedInk-WFC-Slot.md 'BrewedInk.WFC.Slot')  
The slot whose available modules will be returned  
  
#### Returns
[ModuleSet](./BrewedInk-WFC-ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
A set of modules representing all possible modules for the given slot  
