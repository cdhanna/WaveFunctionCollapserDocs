### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[GenerationSpace](./BrewedInk-WFC-GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace(List&lt;BrewedInk.WFC.Slot&gt;, List&lt;BrewedInk.WFC.SlotEdge&gt;, BrewedInk.WFC.ModuleSet, System.Nullable&lt;int&gt;) Constructor
Create a new instance of the WFC algorithm. Each time you construct an instance of the Generation Space, you are setting up a new superposition with nothing collapsed.  
You can also use utility methods to create a new Generation space. [BrewedInk.WFC.GenerationSpace.From2DGrid(System.Int32,System.Int32,BrewedInk.WFC.ModuleSet,System.Nullable{System.Int32},System.Action{System.Collections.Generic.List{BrewedInk.WFC.Slot},System.Collections.Generic.List{BrewedInk.WFC.SlotEdge}})](https://docs.microsoft.com/en-us/dotnet/api/BrewedInk.WFC.GenerationSpace.From2DGrid#BrewedInk_WFC_GenerationSpace_From2DGrid_System_Int32,System_Int32,BrewedInk_WFC_ModuleSet,System_Nullable{System_Int32},System_Action{System_Collections_Generic_List{BrewedInk_WFC_Slot},System_Collections_Generic_List{BrewedInk_WFC_SlotEdge}}_ 'BrewedInk.WFC.GenerationSpace.From2DGrid(System.Int32,System.Int32,BrewedInk.WFC.ModuleSet,System.Nullable{System.Int32},System.Action{System.Collections.Generic.List{BrewedInk.WFC.Slot},System.Collections.Generic.List{BrewedInk.WFC.SlotEdge}})')  
```csharp
public GenerationSpace(List<BrewedInk.WFC.Slot> slots, List<BrewedInk.WFC.SlotEdge> edges, BrewedInk.WFC.ModuleSet allModules, System.Nullable<int> seed);
```
#### Parameters
<a name='BrewedInk-WFC-GenerationSpace-GenerationSpace(List-BrewedInk-WFC-Slot-_List-BrewedInk-WFC-SlotEdge-_BrewedInk-WFC-ModuleSet_System-Nullable-int-)-slots'></a>
`slots` [System.Collections.Generic.List](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List 'System.Collections.Generic.List')  
A set of slots to perform the WFC on. Every slot will be assumed to have every module as a possibility  
  
<a name='BrewedInk-WFC-GenerationSpace-GenerationSpace(List-BrewedInk-WFC-Slot-_List-BrewedInk-WFC-SlotEdge-_BrewedInk-WFC-ModuleSet_System-Nullable-int-)-edges'></a>
`edges` [System.Collections.Generic.List](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List 'System.Collections.Generic.List')  
A set of edges that connect the slots.  
  
<a name='BrewedInk-WFC-GenerationSpace-GenerationSpace(List-BrewedInk-WFC-Slot-_List-BrewedInk-WFC-SlotEdge-_BrewedInk-WFC-ModuleSet_System-Nullable-int-)-allModules'></a>
`allModules` [ModuleSet](./BrewedInk-WFC-ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
A set of all the modules, with the constraints already provided  
  
<a name='BrewedInk-WFC-GenerationSpace-GenerationSpace(List-BrewedInk-WFC-Slot-_List-BrewedInk-WFC-SlotEdge-_BrewedInk-WFC-ModuleSet_System-Nullable-int-)-seed'></a>
`seed` [System.Nullable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Nullable-1 'System.Nullable`1')  
An optional random seed. If you provide the same seed, the WFC algorithm will produce the same output given the same inputs.  
  
