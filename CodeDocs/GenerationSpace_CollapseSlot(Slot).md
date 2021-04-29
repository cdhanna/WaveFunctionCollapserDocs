#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.CollapseSlot(Slot) Method
Given a slot with many module possibilities, collapse the possibility space so that only one module is possible for the given slot.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  
If the given slot has many module possibilities, one module will be selected at random.  
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> CollapseSlot(BrewedInk.WFC.Slot slot);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_CollapseSlot(BrewedInk_WFC_Slot)_slot'></a>
`slot` [Slot](Slot.md 'BrewedInk.WFC.Slot')  
The slot to collapse to a single module possibility
  
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress') representing the completion of the collapse operation. The resulting sequence must be enumerated, or the collapse won't complete. 
