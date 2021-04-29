#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.GenerationSpace(List&lt;Slot&gt;, List&lt;SlotEdge&gt;, ModuleSet, Nullable&lt;int&gt;) Constructor
Create a new instance of the WFC algorithm. Each time you construct an instance of the Generation Space, you are setting up a new superposition with nothing collapsed.  
You can also use utility methods to create a new Generation space. [From2DGrid(int, int, ModuleSet, Nullable&lt;int&gt;, Action&lt;List&lt;Slot&gt;,List&lt;SlotEdge&gt;&gt;)](GenerationSpace_From2DGrid(int_int_ModuleSet_Nullable_int__Action_List_Slot__List_SlotEdge__).md 'BrewedInk.WFC.GenerationSpace.From2DGrid(int, int, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;, System.Action&lt;System.Collections.Generic.List&lt;BrewedInk.WFC.Slot&gt;,System.Collections.Generic.List&lt;BrewedInk.WFC.SlotEdge&gt;&gt;)')
```csharp
public GenerationSpace(System.Collections.Generic.List<BrewedInk.WFC.Slot> slots, System.Collections.Generic.List<BrewedInk.WFC.SlotEdge> edges, BrewedInk.WFC.ModuleSet allModules, System.Nullable<int> seed);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_GenerationSpace(System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__BrewedInk_WFC_ModuleSet_System_Nullable_int_)_slots'></a>
`slots` [System.Collections.Generic.List&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')[Slot](Slot.md 'BrewedInk.WFC.Slot')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')  
A set of slots to perform the WFC on. Every slot will be assumed to have every module as a possibility
  
<a name='BrewedInk_WFC_GenerationSpace_GenerationSpace(System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__BrewedInk_WFC_ModuleSet_System_Nullable_int_)_edges'></a>
`edges` [System.Collections.Generic.List&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')[SlotEdge](SlotEdge.md 'BrewedInk.WFC.SlotEdge')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')  
A set of edges that connect the slots. 
  
<a name='BrewedInk_WFC_GenerationSpace_GenerationSpace(System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__BrewedInk_WFC_ModuleSet_System_Nullable_int_)_allModules'></a>
`allModules` [ModuleSet](ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
A set of all the modules, with the constraints already provided
  
<a name='BrewedInk_WFC_GenerationSpace_GenerationSpace(System_Collections_Generic_List_BrewedInk_WFC_Slot__System_Collections_Generic_List_BrewedInk_WFC_SlotEdge__BrewedInk_WFC_ModuleSet_System_Nullable_int_)_seed'></a>
`seed` [System.Nullable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')  
An optional random seed. If you provide the same seed, the WFC algorithm will produce the same output given the same inputs. 
  
