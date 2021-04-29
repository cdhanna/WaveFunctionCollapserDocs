#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WFCProgressExtensions](WFCProgressExtensions.md 'BrewedInk.WFC.WFCProgressExtensions')
## WFCProgressExtensions.RunAsImmediate(IEnumerable&lt;WFCProgress&gt;, Action&lt;WFCProgress&gt;) Method
Completely iterate through a WFC operation in one frame. Using this method will likely cause lag in your game, and it is only recommended for testing or advanced use.  
```csharp
public static void RunAsImmediate(this System.Collections.Generic.IEnumerable<BrewedInk.WFC.WFCProgress> operation, System.Action<BrewedInk.WFC.WFCProgress> progressHandler=null);
```
#### Parameters
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsImmediate(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__System_Action_BrewedInk_WFC_WFCProgress_)_operation'></a>
`operation` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
Any WFC operation. This could be the return value from any Collapse related function in the [GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
  
<a name='BrewedInk_WFC_WFCProgressExtensions_RunAsImmediate(System_Collections_Generic_IEnumerable_BrewedInk_WFC_WFCProgress__System_Action_BrewedInk_WFC_WFCProgress_)_progressHandler'></a>
`progressHandler` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')  
An optional callback that runs every time a WFCProgress element is processed.
  
