#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')
## WFCProgressObserver.OnSelectedModule&lt;TModule&gt;(Action&lt;Slot,TModule&gt;) Method
A callback that executes anytime a slot collapses to a single module possibility. This is a type of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress'), and will execute right after the [OnProgress(Action&lt;WFCProgress&gt;)](WFCProgressObserver_OnProgress(Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressObserver.OnProgress(System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)') callbacks  
```csharp
public BrewedInk.WFC.WFCProgressObserver OnSelectedModule<TModule>(System.Action<BrewedInk.WFC.Slot,TModule> selection);
```
#### Type parameters
<a name='BrewedInk_WFC_WFCProgressObserver_OnSelectedModule_TModule_(System_Action_BrewedInk_WFC_Slot_TModule_)_TModule'></a>
`TModule`  
the type of module this callback applies for. 
  
#### Parameters
<a name='BrewedInk_WFC_WFCProgressObserver_OnSelectedModule_TModule_(System_Action_BrewedInk_WFC_Slot_TModule_)_selection'></a>
`selection` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')[Slot](Slot.md 'BrewedInk.WFC.Slot')[,](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')[TModule](WFCProgressObserver_OnSelectedModule_TModule_(Action_Slot_TModule_).md#BrewedInk_WFC_WFCProgressObserver_OnSelectedModule_TModule_(System_Action_BrewedInk_WFC_Slot_TModule_)_TModule 'BrewedInk.WFC.WFCProgressObserver.OnSelectedModule&lt;TModule&gt;(System.Action&lt;BrewedInk.WFC.Slot,TModule&gt;).TModule')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-2 'System.Action`2')  
A callback that takes a slot and typed module. This callback only fires when a module of the given type is selected
  
#### Returns
[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')  
The same WFCProgressObserver
