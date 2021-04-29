#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')
## WFCProgressObserver.OnSelectedModule(Action&lt;Slot,Module&gt;) Method
A callback that executes anytime a slot collapses to a single module possibility. This is a type of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress'), and will execute right after the [OnProgress(Action&lt;WFCProgress&gt;)](WFCProgressObserver_OnProgress(Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressObserver.OnProgress(System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)') callbacks  
```csharp
public BrewedInk.WFC.WFCProgressObserver OnSelectedModule(System.Action<BrewedInk.WFC.Slot,BrewedInk.WFC.Module> selection);
```
#### Parameters
<a name='BrewedInk_WFC_WFCProgressObserver_OnSelectedModule(System_Action_BrewedInk_WFC_Slot_BrewedInk_WFC_Module_)_selection'></a>
`selection` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')[Slot](Slot.md 'BrewedInk.WFC.Slot')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')[Module](Module.md 'BrewedInk.WFC.Module')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')  
A callback that takes a slot and a general selection. The module isn't typed, so you'll need to type-check it.
  
#### Returns
[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')  
The same WFCProgressObserver
