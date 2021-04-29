#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.Collapse() Method
Run the WFC algorithm to completion on the Generation Space.  
This method will keep on collapsing the slot with the lowest entropy until all slots have been collapsed to a single module possibility.  
  
This method may take a long time to complete if the Generation Space is large. You should interweave the resulting progress set with a Coroutine with render frames.   
```csharp
public System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> Collapse();
```
#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
A sequence of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress') representing the completion of the collapse operation. The entire sequence must be enumerated or the collapse won't finish.
