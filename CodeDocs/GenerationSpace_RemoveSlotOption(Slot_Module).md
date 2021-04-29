#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.RemoveSlotOption(Slot, Module) Method
A small way to collapse the wave function. At some given slot, this method removes some given module from the set of possible modules at the slot.  
Before this method is run, the given slot may have N possible modules. After the method is run, that slot will have N-1 possible modules.  
This method collapses the superposition at the given slot, which also means that neighboring slots may need to remove modules given the new position.  
This method triggers a propagation event in the Generation Space. As such, it returns a consumable sequence of WFCProgress elements.  
The faster you consume the sequence, the faster the entire propagation phase happens. You may wish to sow render frames between calls. The sequence must be iterated through, or the propagation won't finish.  
  
  
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> RemoveSlotOption(BrewedInk.WFC.Slot startingSlot, BrewedInk.WFC.Module removeModule);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_RemoveSlotOption(BrewedInk_WFC_Slot_BrewedInk_WFC_Module)_startingSlot'></a>
`startingSlot` [Slot](Slot.md 'BrewedInk.WFC.Slot')  
A slot to remove a module option from
  
<a name='BrewedInk_WFC_GenerationSpace_RemoveSlotOption(BrewedInk_WFC_Slot_BrewedInk_WFC_Module)_removeModule'></a>
`removeModule` [Module](Module.md 'BrewedInk.WFC.Module')  
The module to be removed from the slot
  
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress') representing the progress of the propagation event. The sequence must be iterated through, or the propagation won't occur. 
#### Exceptions
[SlotCannotHaveEmptyModuleSetException](SlotCannotHaveEmptyModuleSetException.md 'BrewedInk.WFC.SlotCannotHaveEmptyModuleSetException')  
An exception will be thrown if removing a module from a slot would cause the slot to have zero possible modules. A slot must always have at least one possibility.
