### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[GenerationSpace](./BrewedInk-WFC-GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.CollapseSlot(BrewedInk.WFC.Slot, System.Nullable&lt;int&gt;) Method
Given a slot with many module possibilities, collapse the possibility space so that only one module is possible for the given slot.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  
If the given slot has many module possibilities, one module will be selected at random.  
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> CollapseSlot(BrewedInk.WFC.Slot slot, System.Nullable<int> moduleOffset=null);
```
#### Parameters
<a name='BrewedInk-WFC-GenerationSpace-CollapseSlot(BrewedInk-WFC-Slot_System-Nullable-int-)-slot'></a>
`slot` [Slot](./BrewedInk-WFC-Slot.md 'BrewedInk.WFC.Slot')  
The slot to collapse to a single module possibility  
  
<a name='BrewedInk-WFC-GenerationSpace-CollapseSlot(BrewedInk-WFC-Slot_System-Nullable-int-)-moduleOffset'></a>
`moduleOffset` [System.Nullable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')  
An optional offset to control which module is selected randomly. If there were N modules available, a random number is produced in the range, (0, N]. The moduleOffset is added to the random number, and then the sum is modded by N, producing a number within range. The module that will be selected is found at the modded sum.  
  
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](./BrewedInk-WFC-WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence of [WFCProgress](./BrewedInk-WFC-WFCProgress.md 'BrewedInk.WFC.WFCProgress') representing the completion of the collapse operation. The resulting sequence must be enumerated, or the collapse won't complete.  
