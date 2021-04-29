#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## WFCProgressExtensions Class
A Utility class for IEnumerable sets of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')
```csharp
public static class WFCProgressExtensions
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; WFCProgressExtensions  
### Methods

***
[RunAsCoroutine(IEnumerable&lt;WFCProgress&gt;, MonoBehaviour, float)](WFCProgressExtensions_RunAsCoroutine(IEnumerable_WFCProgress__MonoBehaviour_float).md 'BrewedInk.WFC.WFCProgressExtensions.RunAsCoroutine(System.Collections.Generic.IEnumerable&lt;BrewedInk.WFC.WFCProgress&gt;, UnityEngine.MonoBehaviour, float)')

A method to run any WFC operation within a Unity Coroutine with frame time budgeting. This method will process as many elements in the WFC operation as possible in on frame, then yield a render frame, and continue the operation on the next frame.  
This is the recommended way to run WFC operations in a realtime game.  
This returns a [WFCProgressObserver](WFCProgressObserver.md 'BrewedInk.WFC.WFCProgressObserver') object which you can attach progress callbacks and inspect the running state.  

***
[RunAsImmediate(IEnumerable&lt;WFCProgress&gt;, Action&lt;WFCProgress&gt;)](WFCProgressExtensions_RunAsImmediate(IEnumerable_WFCProgress__Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressExtensions.RunAsImmediate(System.Collections.Generic.IEnumerable&lt;BrewedInk.WFC.WFCProgress&gt;, System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)')

Completely iterate through a WFC operation in one frame. Using this method will likely cause lag in your game, and it is only recommended for testing or advanced use.  
