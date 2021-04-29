#### [brewkedink.wfc](index.md 'index')
### [](.md '')
## WCFConfigObject&lt;TModuleObject,TModule&gt; Class
```csharp
public abstract class WCFConfigObject<TModuleObject,TModule> : global::WCFConfigObject
    where TModuleObject : global::ModuleObject<TModule>
    where TModule : BrewedInk.WFC.Module
```
#### Type parameters
<a name='WCFConfigObject_TModuleObject_TModule__TModuleObject'></a>
`TModuleObject`  
  
<a name='WCFConfigObject_TModuleObject_TModule__TModule'></a>
`TModule`  
  

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [UnityEngine.Object](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.Object 'UnityEngine.Object') &#129106; [UnityEngine.ScriptableObject](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.ScriptableObject 'UnityEngine.ScriptableObject') &#129106; [WCFConfigObject](WCFConfigObject.md 'WCFConfigObject') &#129106; WCFConfigObject&lt;TModuleObject,TModule&gt;  

Derived  
&#8627; [SpriteConfig](SpriteConfig.md 'SpriteConfig')  
### Fields

***
[seed](WCFConfigObject_TModuleObject_TModule__seed.md 'global::WCFConfigObject&lt;TModuleObject,TModule&gt;.seed')

If the useSeed boolean is true, what seed should be used? This property should be ignored if useSeed is false.  

***
[useSeed](WCFConfigObject_TModuleObject_TModule__useSeed.md 'global::WCFConfigObject&lt;TModuleObject,TModule&gt;.useSeed')

Should the [GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace') instances that this instance creates use a seed?/>  
### Methods

***
[CreateSpace(ModuleSet)](WCFConfigObject_TModuleObject_TModule__CreateSpace(ModuleSet).md 'global::WCFConfigObject&lt;TModuleObject,TModule&gt;.CreateSpace(BrewedInk.WFC.ModuleSet)')

You need to create a Generation Space given a set of user defined modules and configuration.   

***
[TryGetObject(Module, TModuleObject)](WCFConfigObject_TModuleObject_TModule__TryGetObject(Module_TModuleObject).md 'global::WCFConfigObject&lt;TModuleObject,TModule&gt;.TryGetObject(BrewedInk.WFC.Module, TModuleObject)')

Given the typeless Module, get the wrapper object for it. The wrapper object may have additional metadata about the module that isn't used in the WFC algorithm, but may be useful for other parts of the game.  
