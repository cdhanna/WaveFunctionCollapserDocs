#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.CollapseLowestEntropySlot() Method
Collapse the superposition of some slot. The slot that is selected is the slot in the Generation Space with the lowest entropy. A Slot's entropy is found by taking the count of available modules remaining at the slot.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  
By default, WFC always prefer to collapse the slot with the lowest entropy, because it is less likely to produce an invalid outcome.  
  
If there are multiple slots with the same entropy, the first one detected in the Generation Space's internal data structure will be used. It is not random. It depends on how the slots were created in the constructor of the Generation Space.  
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> CollapseLowestEntropySlot();
```
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
