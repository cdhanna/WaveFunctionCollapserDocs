#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## GenerationSpace Class
The Generation Space is the main access point for the WFC algorithm. The Generation Space holds a directed graph of Slots, and a set of all possible modules per slot.  
The Generation Space has methods for collapsing the superposition of the Slots, until all slots only have one module option left.  
```csharp
public class GenerationSpace
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; GenerationSpace  
### Constructors

***
[GenerationSpace(List&lt;Slot&gt;, List&lt;SlotEdge&gt;, ModuleSet, Nullable&lt;int&gt;)](GenerationSpace_GenerationSpace(List_Slot__List_SlotEdge__ModuleSet_Nullable_int_).md 'BrewedInk.WFC.GenerationSpace.GenerationSpace(System.Collections.Generic.List&lt;BrewedInk.WFC.Slot&gt;, System.Collections.Generic.List&lt;BrewedInk.WFC.SlotEdge&gt;, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;)')

Create a new instance of the WFC algorithm. Each time you construct an instance of the Generation Space, you are setting up a new superposition with nothing collapsed.  
You can also use utility methods to create a new Generation space. [From2DGrid(int, int, ModuleSet, Nullable&lt;int&gt;, Action&lt;List&lt;Slot&gt;,List&lt;SlotEdge&gt;&gt;)](GenerationSpace_From2DGrid(int_int_ModuleSet_Nullable_int__Action_List_Slot__List_SlotEdge__).md 'BrewedInk.WFC.GenerationSpace.From2DGrid(int, int, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;, System.Action&lt;System.Collections.Generic.List&lt;BrewedInk.WFC.Slot&gt;,System.Collections.Generic.List&lt;BrewedInk.WFC.SlotEdge&gt;&gt;)')
### Methods

***
[Collapse()](GenerationSpace_Collapse().md 'BrewedInk.WFC.GenerationSpace.Collapse()')

Run the WFC algorithm to completion on the Generation Space.  
This method will keep on collapsing the slot with the lowest entropy until all slots have been collapsed to a single module possibility.  
  
This method may take a long time to complete if the Generation Space is large. You should interweave the resulting progress set with a Coroutine with render frames.   

***
[CollapseLowestEntropySlot()](GenerationSpace_CollapseLowestEntropySlot().md 'BrewedInk.WFC.GenerationSpace.CollapseLowestEntropySlot()')

Collapse the superposition of some slot. The slot that is selected is the slot in the Generation Space with the lowest entropy. A Slot's entropy is found by taking the count of available modules remaining at the slot.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  
By default, WFC always prefer to collapse the slot with the lowest entropy, because it is less likely to produce an invalid outcome.  
  
If there are multiple slots with the same entropy, the first one detected in the Generation Space's internal data structure will be used. It is not random. It depends on how the slots were created in the constructor of the Generation Space.  

***
[CollapseSlot(Slot, Module)](GenerationSpace_CollapseSlot(Slot_Module).md 'BrewedInk.WFC.GenerationSpace.CollapseSlot(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)')

Collapse a slot to a given module outcome.  
If a slot had N possible modules, after this method runs, the slot would only have 1 possible module.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  

***
[CollapseSlot(Slot)](GenerationSpace_CollapseSlot(Slot).md 'BrewedInk.WFC.GenerationSpace.CollapseSlot(BrewedInk.WFC.Slot)')

Given a slot with many module possibilities, collapse the possibility space so that only one module is possible for the given slot.  
This will cause many propagation events, and may cause other slots to collapse to a single module possibility as well.  
If the given slot has many module possibilities, one module will be selected at random.  

***
[From2DGrid(int, int, ModuleSet, Nullable&lt;int&gt;, Action&lt;List&lt;Slot&gt;,List&lt;SlotEdge&gt;&gt;)](GenerationSpace_From2DGrid(int_int_ModuleSet_Nullable_int__Action_List_Slot__List_SlotEdge__).md 'BrewedInk.WFC.GenerationSpace.From2DGrid(int, int, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;, System.Action&lt;System.Collections.Generic.List&lt;BrewedInk.WFC.Slot&gt;,System.Collections.Generic.List&lt;BrewedInk.WFC.SlotEdge&gt;&gt;)')

A utility method for building a Generation Space in the form of a 2D grid.  
All Generation Spaces are directed graphs, and the resulting Generation Space from this method will be a graph representing a 2D grid. Each cell in the grid will have neighbors to the west, east, south, and north. There are no diagonal neighbors.  

***
[GetEdges(Slot)](GenerationSpace_GetEdges(Slot).md 'BrewedInk.WFC.GenerationSpace.GetEdges(BrewedInk.WFC.Slot)')

Get a Slot's edges.  
[SlotEdge](SlotEdge.md 'BrewedInk.WFC.SlotEdge')

***
[GetEntropy(ModuleSet)](GenerationSpace_GetEntropy(ModuleSet).md 'BrewedInk.WFC.GenerationSpace.GetEntropy(BrewedInk.WFC.ModuleSet)')

Calculates the entropy of a set of modules.  
Entropy is ```csharp
 -sum(p log(p) )```
 over all modules where each p is the probability of the module  

***
[GetEntropy(Slot)](GenerationSpace_GetEntropy(Slot).md 'BrewedInk.WFC.GenerationSpace.GetEntropy(BrewedInk.WFC.Slot)')

Calculates the current entropy of a slot.  
Entropy is roughly equal to the number of modules left in the slot's wave function. The contribution of each module is weighted by the module's weight. [Weight](Module_Weight.md 'BrewedInk.WFC.Module.Weight')  
The exact entropy calculation is ```csharp
 -sum( p log(p) ) ```
 over all modules where each p is the probability of the module.   

***
[GetSlot(Vector3Int)](GenerationSpace_GetSlot(Vector3Int).md 'BrewedInk.WFC.GenerationSpace.GetSlot(UnityEngine.Vector3Int)')

Find a slot given a position. If no slot exists at the given position, this method will return null.  

***
[GetSlotOptions(Slot)](GenerationSpace_GetSlotOptions(Slot).md 'BrewedInk.WFC.GenerationSpace.GetSlotOptions(BrewedInk.WFC.Slot)')

At any given moment, a slot may have many possible modules available to it. This method will give you the set of possible modules available on a slot.  

***
[RemoveSlotOption(Slot, Module)](GenerationSpace_RemoveSlotOption(Slot_Module).md 'BrewedInk.WFC.GenerationSpace.RemoveSlotOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)')

A small way to collapse the wave function. At some given slot, this method removes some given module from the set of possible modules at the slot.  
Before this method is run, the given slot may have N possible modules. After the method is run, that slot will have N-1 possible modules.  
This method collapses the superposition at the given slot, which also means that neighboring slots may need to remove modules given the new position.  
This method triggers a propagation event in the Generation Space. As such, it returns a consumable sequence of WFCProgress elements.  
The faster you consume the sequence, the faster the entire propagation phase happens. You may wish to sow render frames between calls. The sequence must be iterated through, or the propagation won't finish.  
  
  

***
[Reset()](GenerationSpace_Reset().md 'BrewedInk.WFC.GenerationSpace.Reset()')

Reset all slot superpositions so that all modules are likely again.   

***
[TryGetOnlyOption(Slot, Module)](GenerationSpace_TryGetOnlyOption(Slot_Module).md 'BrewedInk.WFC.GenerationSpace.TryGetOnlyOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module)')

At any given moment, a slot may have many possible modules available to it. However, eventually, a slot will only have one possible module remaining.  
This method will help you identify when there is only one module left per slot.  
If there is only one module left for the given slot, this method will return true and store the assigned module in the out parameter. If there is more than one module possible, the method will return false, and the out variable will be null.  
  
You can also retrieve all of the available slot modules with the ` GenerationSpace.GetSlotOptions ` method.  
[GetSlotOptions(Slot)](GenerationSpace_GetSlotOptions(Slot).md 'BrewedInk.WFC.GenerationSpace.GetSlotOptions(BrewedInk.WFC.Slot)')

***
[Validate()](GenerationSpace_Validate().md 'BrewedInk.WFC.GenerationSpace.Validate()')

Evaluate all constraints in the Generation Space and return the number if invalid constraints.  
Ideally, this method should always return zero. However, you can use this to check that the constraints are indeed valid if  
you suspect that the collapse has errored.   
