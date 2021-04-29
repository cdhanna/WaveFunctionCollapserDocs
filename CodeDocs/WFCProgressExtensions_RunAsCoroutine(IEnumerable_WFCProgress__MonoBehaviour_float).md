#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressExtensions](WFCProgressExtensions.md 'BrewedInk.WFC.WFCProgressExtensions')
## WFCProgressExtensions.RunAsCoroutine(IEnumerable&lt;WFCProgress&gt;, MonoBehaviour, float) Method
A method to run any WFC operation within a Unity Coroutine with frame time budgeting. This method will process as many elements in the WFC operation as possible in on frame, then yield a render frame, and continue the operation on the next frame.  
This is the recommended way to run WFC operations in a realtime game.  
This returns a [WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver') object which you can attach progress callbacks and inspect the running state.  
```csharp
public static BrewedInk.WFC.WFCProgressObserver RunAsCoroutine(this System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> operation, UnityEngine.MonoBehaviour context, float timeBudgetPerFrame=0.1f);
```
#### Parameters
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float)_operation'></a>
`operation` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
Any WFC operation. This could be the return value from any Collapse related function in the [GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
  
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float)_context'></a>
`context` [UnityEngine.MonoBehaviour](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.MonoBehaviour 'UnityEngine.MonoBehaviour')  
Some Monobehaviour to run the Coroutine in.
  
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float)_timeBudgetPerFrame'></a>
`timeBudgetPerFrame` [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single')  
How much is available per frame to operate on the WFC sequence? This should be a low number, so that it doesn't cause hitches in your game.
  
#### Returns
[WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver')  
a WFCProgressObserver
