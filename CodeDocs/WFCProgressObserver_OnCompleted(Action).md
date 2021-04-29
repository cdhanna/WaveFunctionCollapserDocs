#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')
## WFCProgressObserver.OnCompleted(Action) Method
A callback that executes when the WFC operation has completed. This happens right after the [WFCProgressObserver.OnComplete](https://docs.microsoft.com/en-us/dotnet/api/WFCProgressObserver.OnComplete 'WFCProgressObserver.OnComplete') is set to true.  
```csharp
public BrewedInk.WFC.WFCProgressObserver OnCompleted(System.Action onComplete);
```
#### Parameters
<a name='BrewedInk_WFC_WFCProgressObserver_OnCompleted(System_Action)_onComplete'></a>
`onComplete` [System.Action](https://docs.microsoft.com/en-us/dotnet/api/System.Action 'System.Action')  
a callback to run on completion
  
#### Returns
[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')  
The same WFCProgressObserver
