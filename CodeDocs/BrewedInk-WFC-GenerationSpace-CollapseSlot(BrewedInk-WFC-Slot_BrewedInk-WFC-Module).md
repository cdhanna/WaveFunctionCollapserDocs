### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[GenerationSpace](./BrewedInk-WFC-GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.CollapseSlot(BrewedInk.WFC.Slot, BrewedInk.WFC.Module) Method
Collapse a slot to a given module outcome.  
If a slot had N possible modules, after this method runs, the slot would only have 1 possible module.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> CollapseSlot(BrewedInk.WFC.Slot slot, BrewedInk.WFC.Module module);
```
#### Parameters
<a name='BrewedInk-WFC-GenerationSpace-CollapseSlot(BrewedInk-WFC-Slot_BrewedInk-WFC-Module)-slot'></a>
`slot` [Slot](./BrewedInk-WFC-Slot.md 'BrewedInk.WFC.Slot')  
A slot to collapse to one module possibility  
  
<a name='BrewedInk-WFC-GenerationSpace-CollapseSlot(BrewedInk-WFC-Slot_BrewedInk-WFC-Module)-module'></a>
`module` [Module](./BrewedInk-WFC-Module.md 'BrewedInk.WFC.Module')  
the module that will be only remaining possibility for the given slot  
  
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](./BrewedInk-WFC-WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence of [WFCProgress](./BrewedInk-WFC-WFCProgress.md 'BrewedInk.WFC.WFCProgress') representing the progress of the collapse operation. The sequence must be enumerated, or the collapse won't finish.  
#### Exceptions
[SlotCannotSelectUnavailableModule](./BrewedInk-WFC-SlotCannotSelectUnavailableModule.md 'BrewedInk.WFC.SlotCannotSelectUnavailableModule')  
You cannot select a module for a slot if the slot doesn't already contain the module in its superposition.  
