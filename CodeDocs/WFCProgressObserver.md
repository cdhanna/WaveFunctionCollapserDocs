#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## WFCProgressObserver Class
A wrapper class around the invocation of a WFC collapse operation.  
You should use this in conjunction with [RunAsCoroutine(IEnumerable&lt;WFCProgress&gt;, MonoBehaviour, float)](WFCProgressExtensions_RunAsCoroutine(IEnumerable_WFCProgress__MonoBehaviour_float).md 'BrewedInk.WFC.WFCProgressExtensions.RunAsCoroutine(System.Collections.Generic.IEnumerable&lt;BrewedInk.WFC.WFCProgress&gt;, UnityEngine.MonoBehaviour, float)')
```csharp
public class WFCProgressObserver
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; WFCProgressObserver  
### Properties

***
[IsComplete](WFCProgressObserver_IsComplete.md 'BrewedInk.WFC.WFCProgressObserver.IsComplete')

Returns true when the operation is complete. This will be true the instant BEFORE the onComplete callbacks are invoked.  

***
[ProgressCount](WFCProgressObserver_ProgressCount.md 'BrewedInk.WFC.WFCProgressObserver.ProgressCount')

The number of progress events received for this operation. There isn't a knowable upper bound, but you can use this to track that progress is happening.  

***
[SlotSelections](WFCProgressObserver_SlotSelections.md 'BrewedInk.WFC.WFCProgressObserver.SlotSelections')

A set of selections you can use inspect to see what has finished. If you want an event driven approach, use [OnSelectedModule(Action&lt;SlotModuleSelected&gt;)](WFCProgressObserver_OnSelectedModule(Action_SlotModuleSelected_).md 'BrewedInk.WFC.WFCProgressObserver.OnSelectedModule(System.Action&lt;BrewedInk.WFC.SlotModuleSelected&gt;)')
### Methods

***
[OnCompleted(Action)](WFCProgressObserver_OnCompleted(Action).md 'BrewedInk.WFC.WFCProgressObserver.OnCompleted(System.Action)')

A callback that executes when the WFC operation has completed. This happens right after the [WFCProgressObserver.OnComplete](https://docs.microsoft.com/en-us/dotnet/api/WFCProgressObserver.OnComplete 'WFCProgressObserver.OnComplete') is set to true.  

***
[OnProgress(Action&lt;WFCProgress&gt;)](WFCProgressObserver_OnProgress(Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressObserver.OnProgress(System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)')

A callback that executes anytime the WFC has new progress. Progress elements can represent a module being removed, or a module being selected, an error, or a general propagation of data.  

***
[OnSelectedModule(Action&lt;Slot,Module&gt;)](WFCProgressObserver_OnSelectedModule(Action_Slot_Module_).md 'BrewedInk.WFC.WFCProgressObserver.OnSelectedModule(System.Action&lt;BrewedInk.WFC.Slot,BrewedInk.WFC.Module&gt;)')

A callback that executes anytime a slot collapses to a single module possibility. This is a type of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress'), and will execute right after the [OnProgress(Action&lt;WFCProgress&gt;)](WFCProgressObserver_OnProgress(Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressObserver.OnProgress(System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)') callbacks  

***
[OnSelectedModule(Action&lt;SlotModuleSelected&gt;)](WFCProgressObserver_OnSelectedModule(Action_SlotModuleSelected_).md 'BrewedInk.WFC.WFCProgressObserver.OnSelectedModule(System.Action&lt;BrewedInk.WFC.SlotModuleSelected&gt;)')

A callback that executes anytime a slot collapses to a single module possibility. This is a type of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress'), and will execute right after the [OnProgress(Action&lt;WFCProgress&gt;)](WFCProgressObserver_OnProgress(Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressObserver.OnProgress(System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)') callbacks  

***
[OnSelectedModule&lt;TModule&gt;(Action&lt;Slot,TModule&gt;)](WFCProgressObserver_OnSelectedModule_TModule_(Action_Slot_TModule_).md 'BrewedInk.WFC.WFCProgressObserver.OnSelectedModule&lt;TModule&gt;(System.Action&lt;BrewedInk.WFC.Slot,TModule&gt;)')

A callback that executes anytime a slot collapses to a single module possibility. This is a type of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress'), and will execute right after the [OnProgress(Action&lt;WFCProgress&gt;)](WFCProgressObserver_OnProgress(Action_WFCProgress_).md 'BrewedInk.WFC.WFCProgressObserver.OnProgress(System.Action&lt;BrewedInk.WFC.WFCProgress&gt;)') callbacks  
