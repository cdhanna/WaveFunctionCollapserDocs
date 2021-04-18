### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC')
## GenerationSpace Class
The Generation Space is the main access point for the WFC algorithm. The Generation Space holds a directed graph of Slots, and a set of all possible modules per slot.  
The Generation Space has methods for collapsing the superposition of the Slots, until all slots only have one module option left.  
```csharp
public class GenerationSpace
```
Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; GenerationSpace  
### Constructors
- [GenerationSpace(List&lt;BrewedInk.WFC.Slot&gt;, List&lt;BrewedInk.WFC.SlotEdge&gt;, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;)](./BrewedInk-WFC-GenerationSpace-GenerationSpace(List-BrewedInk-WFC-Slot-_List-BrewedInk-WFC-SlotEdge-_BrewedInk-WFC-ModuleSet_System-Nullable-int-).md 'BrewedInk.WFC.GenerationSpace.GenerationSpace(List&lt;BrewedInk.WFC.Slot&gt;, List&lt;BrewedInk.WFC.SlotEdge&gt;, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;)')
### Methods
- [Collapse()](./BrewedInk-WFC-GenerationSpace-Collapse().md 'BrewedInk.WFC.GenerationSpace.Collapse()')
- [CollapseLowestEntropySlot()](./BrewedInk-WFC-GenerationSpace-CollapseLowestEntropySlot().md 'BrewedInk.WFC.GenerationSpace.CollapseLowestEntropySlot()')
- [CollapseSlot(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)](./BrewedInk-WFC-GenerationSpace-CollapseSlot(BrewedInk-WFC-Slot_BrewedInk-WFC-Module).md 'BrewedInk.WFC.GenerationSpace.CollapseSlot(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)')
- [CollapseSlot(BrewedInk.WFC.Slot, System.Nullable&lt;int&gt;)](./BrewedInk-WFC-GenerationSpace-CollapseSlot(BrewedInk-WFC-Slot_System-Nullable-int-).md 'BrewedInk.WFC.GenerationSpace.CollapseSlot(BrewedInk.WFC.Slot, System.Nullable&lt;int&gt;)')
- [From2DGrid(int, int, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;, Action&lt;List&lt;BrewedInk.WFC.Slot&gt;,List&lt;BrewedInk.WFC.SlotEdge&gt;&gt;)](./BrewedInk-WFC-GenerationSpace-From2DGrid(int_int_BrewedInk-WFC-ModuleSet_System-Nullable-int-_Action-List-BrewedInk-WFC-Slot-_List-BrewedInk-WFC-SlotEdge--).md 'BrewedInk.WFC.GenerationSpace.From2DGrid(int, int, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;, Action&lt;List&lt;BrewedInk.WFC.Slot&gt;,List&lt;BrewedInk.WFC.SlotEdge&gt;&gt;)')
- [GetEdges(BrewedInk.WFC.Slot)](./BrewedInk-WFC-GenerationSpace-GetEdges(BrewedInk-WFC-Slot).md 'BrewedInk.WFC.GenerationSpace.GetEdges(BrewedInk.WFC.Slot)')
- [GetSlot(UnityEngine.Vector3Int)](./BrewedInk-WFC-GenerationSpace-GetSlot(UnityEngine-Vector3Int).md 'BrewedInk.WFC.GenerationSpace.GetSlot(UnityEngine.Vector3Int)')
- [GetSlotOptions(BrewedInk.WFC.Slot)](./BrewedInk-WFC-GenerationSpace-GetSlotOptions(BrewedInk-WFC-Slot).md 'BrewedInk.WFC.GenerationSpace.GetSlotOptions(BrewedInk.WFC.Slot)')
- [RemoveSlotOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)](./BrewedInk-WFC-GenerationSpace-RemoveSlotOption(BrewedInk-WFC-Slot_BrewedInk-WFC-Module).md 'BrewedInk.WFC.GenerationSpace.RemoveSlotOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)')
- [Reset()](./BrewedInk-WFC-GenerationSpace-Reset().md 'BrewedInk.WFC.GenerationSpace.Reset()')
- [TryGetOnlyOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)](./BrewedInk-WFC-GenerationSpace-TryGetOnlyOption(BrewedInk-WFC-Slot_BrewedInk-WFC-Module).md 'BrewedInk.WFC.GenerationSpace.TryGetOnlyOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)')
