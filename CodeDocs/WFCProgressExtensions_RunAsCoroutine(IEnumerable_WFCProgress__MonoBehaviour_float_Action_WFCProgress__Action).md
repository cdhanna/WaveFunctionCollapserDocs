### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressExtensions](WFCProgressExtensions.md 'BrewedInk.WFC.WFCProgressExtensions')
## WFCProgressExtensions.RunAsCoroutine(IEnumerable&lt;WFCProgress&gt;, MonoBehaviour, float, Action&lt;WFCProgress&gt;, Action) Method
A method to run any WFC operation within a Unity Coroutine with frame time budgeting. This method will process as many elements in the WFC operation as possible in on frame, then yield a render frame, and continue the operation on the next frame.  
This is the recommended way to run WFC operations in a realtime game.  
```csharp
public static UnityEngine.Coroutine RunAsCoroutine(this System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> operation, UnityEngine.MonoBehaviour context, float timeBudgetPerFrame, System.Action<BrewedInk.WFC.WFCProgress> onProgress=null, System.Action onCompleted=null);
```
#### Parameters
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float_System_Action_BrewedInk_WFC_WFCProgress__System_Action)_operation'></a>
`operation` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
Any WFC operation. This could be the return value from any Collapse related function in the [GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
  
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float_System_Action_BrewedInk_WFC_WFCProgress__System_Action)_context'></a>
`context` [UnityEngine.MonoBehaviour](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.MonoBehaviour 'UnityEngine.MonoBehaviour')  
Some Monobehaviour to run the Coroutine in.
  
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float_System_Action_BrewedInk_WFC_WFCProgress__System_Action)_timeBudgetPerFrame'></a>
`timeBudgetPerFrame` [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single')  
How much is available per frame to operate on the WFC sequence? This should be a low number, so that it doesn't cause hitches in your game.
  
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float_System_Action_BrewedInk_WFC_WFCProgress__System_Action)_onProgress'></a>
`onProgress` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')  
An optional callback that runs every time a WFCProgress element is processed.
  
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsCoroutine(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__UnityEngine_MonoBehaviour_float_System_Action_BrewedInk_WFC_WFCProgress__System_Action)_onCompleted'></a>
`onCompleted` [System.Action](https://docs.microsoft.com/en-us/dotnet/api/System.Action 'System.Action')  
An optional callback that runs when the Coroutine has finished processing the WFC operation
  
#### Returns
[UnityEngine.Coroutine](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.Coroutine 'UnityEngine.Coroutine')  
