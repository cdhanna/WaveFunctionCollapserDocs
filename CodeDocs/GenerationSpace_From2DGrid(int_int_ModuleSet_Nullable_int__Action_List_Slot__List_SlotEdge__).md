#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.From2DGrid(int, int, ModuleSet, Nullable&lt;int&gt;, Action&lt;List&lt;Slot&gt;,List&lt;SlotEdge&gt;&gt;) Method
A utility method for building a Generation Space in the form of a 2D grid.  
All Generation Spaces are directed graphs, and the resulting Generation Space from this method will be a graph representing a 2D grid. Each cell in the grid will have neighbors to the west, east, south, and north. There are no diagonal neighbors.  
```csharp
public static BrewedInk.WFC.GenerationSpace From2DGrid(int width, int height, BrewedInk.WFC.ModuleSet modules, System.Nullable<int> seed=null, System.Action<System.Collections.Generic.List<BrewedInk.WFC.Slot>,System.Collections.Generic.List<BrewedInk.WFC.SlotEdge>> prepareSpace=null);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_From2DGrid(int_int_BrewedInk_WFC_ModuleSet_System_Nullable_int__System_Action_System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__)_width'></a>
`width` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')  
The width of the resulting 2D grid Generation Space
  
<a name='BrewedInk_WFC_GenerationSpace_From2DGrid(int_int_BrewedInk_WFC_ModuleSet_System_Nullable_int__System_Action_System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__)_height'></a>
`height` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')  
The height of the resulting 2D grid Generation Space
  
<a name='BrewedInk_WFC_GenerationSpace_From2DGrid(int_int_BrewedInk_WFC_ModuleSet_System_Nullable_int__System_Action_System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__)_modules'></a>
`modules` [ModuleSet](ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
The set of all possible modules, with constraints prepopulated. Every Slot that is created in this Generation Space will have all modules available at the start of the WFC.
  
<a name='BrewedInk_WFC_GenerationSpace_From2DGrid(int_int_BrewedInk_WFC_ModuleSet_System_Nullable_int__System_Action_System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__)_seed'></a>
`seed` [System.Nullable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')  
An optional seed that controls how the WFC decides random operations. 
  
<a name='BrewedInk_WFC_GenerationSpace_From2DGrid(int_int_BrewedInk_WFC_ModuleSet_System_Nullable_int__System_Action_System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__)_prepareSpace'></a>
`prepareSpace` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')[System.Collections.Generic.List&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')[Slot](Slot.md 'BrewedInk.WFC.Slot')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')[System.Collections.Generic.List&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')[SlotEdge](SlotEdge.md 'BrewedInk.WFC.SlotEdge')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')  
An optional callback to control how edges are created in the 2D grid. If this parameter is left null, every slot will have edges to the west, east, south, and north. If you need to change how the edges are created, remove certain edges, or add additional edges, you can provide your own implementation of this callback. If you provide a callback value, you are responsible for populating the entire List of SlotEdges per given Slot.
  
#### Returns
[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')  
A Generation Space representing a 2D grid of slots where every slot has every module available to it at the start of the WFC. 
