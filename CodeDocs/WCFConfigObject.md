#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## WCFConfigObject Class
A ScriptableObject wrapper that streamlines creating [GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace') instances from MonoBehaviours.   
```csharp
public abstract class WCFConfigObject : UnityEngine.ScriptableObject
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [UnityEngine.Object](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.Object 'UnityEngine.Object') &#129106; [UnityEngine.ScriptableObject](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.ScriptableObject 'UnityEngine.ScriptableObject') &#129106; WCFConfigObject  

Derived  
&#8627; [WCFConfigObject&lt;TModuleObject,TModule&gt;](WCFConfigObject_TModuleObject_TModule_.md 'BrewedInk.WFC.WCFConfigObject&lt;TModuleObject,TModule&gt;')  
### Methods

***
[Create()](WCFConfigObject_Create().md 'BrewedInk.WFC.WCFConfigObject.Create()')

Create a blank [GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace') from the configuration.  
This is a useful method for creating generation spaces pre-configured with edges, slots, and modules.  

***
[TryGetSprite(Module, Sprite)](WCFConfigObject_TryGetSprite(Module_Sprite).md 'BrewedInk.WFC.WCFConfigObject.TryGetSprite(BrewedInk.WFC.Module, UnityEngine.Sprite)')

If a module has a Sprite associated with it, you can use this method to try and get it. Depending on the type of Module, there may not be any Sprite available.   
