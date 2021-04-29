#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')
## WFCProgressObserver.OnSelectedModule(Action&lt;SlotModuleSelected&gt;) Method
A callback that executes anytime a slot collapses to a single module possibility. This is a type of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress'), and will execute right after the [OnProgress(Action&lt;WFCProgress&gt;)](WFCProgressObserver_OnProgress(Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressObserver.OnProgress(System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)') callbacks  
```csharp
public BrewedInk.WFC.WFCProgressObserver OnSelectedModule(System.Action<BrewedInk.WFC.SlotModuleSelected> selection);
```
#### Parameters
<a name='BrewedInk_WFC_WFCProgressObserver_OnSelectedModule(System_Action_BrewedInk_WFC_SlotModuleSelected_)_selection'></a>
`selection` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[SlotModuleSelected](SlotModuleSelected.md 'BrewedInk.WFC.SlotModuleSelected')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')  
A callback that takes a general selection. The module isn't typed, so you'll need to type-check it.
  
#### Returns
[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')  
The same WFCProgressObserver
