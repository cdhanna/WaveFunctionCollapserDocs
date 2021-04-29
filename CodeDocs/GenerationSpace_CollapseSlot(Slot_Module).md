#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.CollapseSlot(Slot, Module) Method
Collapse a slot to a given module outcome.  
If a slot had N possible modules, after this method runs, the slot would only have 1 possible module.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> CollapseSlot(BrewedInk.WFC.Slot slot, BrewedInk.WFC.Module module);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_CollapseSlot(BrewedInk_WFC_Slot_BrewedInk_WFC_Module)_slot'></a>
`slot` [Slot](Slot.md 'BrewedInk.WFC.Slot')  
A slot to collapse to one module possibility
  
<a name='BrewedInk_WFC_GenerationSpace_CollapseSlot(BrewedInk_WFC_Slot_BrewedInk_WFC_Module)_module'></a>
`module` [Module](Module.md 'BrewedInk.WFC.Module')  
the module that will be only remaining possibility for the given slot
  
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress') representing the progress of the collapse operation. The sequence must be enumerated, or the collapse won't finish.
#### Exceptions
[SlotCannotSelectUnavailableModule](SlotCannotSelectUnavailableModule.md 'BrewedInk.WFC.SlotCannotSelectUnavailableModule')  
You cannot select a module for a slot if the slot doesn't already contain the module in its superposition. 
