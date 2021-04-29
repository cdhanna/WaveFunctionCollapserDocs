#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')
## WFCProgressObserver.OnProgress(Action&lt;WFCProgress&gt;) Method
A callback that executes anytime the WFC has new progress. Progress elements can represent a module being removed, or a module being selected, an error, or a general propagation of data.  
```csharp
public BrewedInk.WFC.WFCProgressObserver OnProgress(System.Action<BrewedInk.WFC.WFCProgress> onProgress);
```
#### Parameters
<a name='BrewedInk_WFC_WFCProgressObserver_OnProgress(System_Action_BrewedInk_WFC_WFCProgress_)_onProgress'></a>
`onProgress` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')  
A callback to run on progress
  
#### Returns
[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')  
The same WFCProgressObserver
