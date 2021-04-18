### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[GenerationSpace](./BrewedInk-WFC-GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.RemoveSlotOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module) Method
A small way to collapse the wave function. At some given slot, this method removes some given module from the set of possible modules at the slot.  
Before this method is run, the given slot may have N possible modules. After the method is run, that slot will have N-1 possible modules.  
This method collapses the superposition at the given slot, which also means that neighboring slots may need to remove modules given the new position.  
This method triggers a propagation event in the Generation Space. As such, it returns a consumable sequence of WFCProgress elements.  
The faster you consume the sequence, the faster the entire propagation phase happens. You may wish to sow render frames between calls. The sequence must be iterated through, or the propagation won't finish.  
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> RemoveSlotOption(BrewedInk.WFC.Slot startingSlot, BrewedInk.WFC.Module removeModule);
```
#### Parameters
<a name='BrewedInk-WFC-GenerationSpace-RemoveSlotOption(BrewedInk-WFC-Slot_BrewedInk-WFC-Module)-startingSlot'></a>
`startingSlot` [Slot](./BrewedInk-WFC-Slot.md 'BrewedInk.WFC.Slot')  
A slot to remove a module option from  
  
<a name='BrewedInk-WFC-GenerationSpace-RemoveSlotOption(BrewedInk-WFC-Slot_BrewedInk-WFC-Module)-removeModule'></a>
`removeModule` [Module](./BrewedInk-WFC-Module.md 'BrewedInk.WFC.Module')  
The module to be removed from the slot  
  
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](./BrewedInk-WFC-WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence of [WFCProgress](./BrewedInk-WFC-WFCProgress.md 'BrewedInk.WFC.WFCProgress') representing the progress of the propagation event. The sequence must be iterated through, or the propagation won't occur.  
#### Exceptions
[SlotCannotHaveEmptyModuleSetException](./BrewedInk-WFC-SlotCannotHaveEmptyModuleSetException.md 'BrewedInk.WFC.SlotCannotHaveEmptyModuleSetException')  
An exception will be thrown if removing a module from a slot would cause the slot to have zero possible modules. A slot must always have at least one possibility.  
