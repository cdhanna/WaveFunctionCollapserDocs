#### [brewkedink.wfc](index.md 'index')
### [](.md '').[WCFConfigObject&lt;TModuleObject,TModule&gt;](WCFConfigObject_TModuleObject_TModule_.md 'WCFConfigObject&lt;TModuleObject,TModule&gt;')
## WCFConfigObject&lt;TModuleObject,TModule&gt;.CreateSpace(ModuleSet) Method
You need to create a Generation Space given a set of user defined modules and configuration.   
```csharp
protected abstract BrewedInk.WFC.GenerationSpace CreateSpace(BrewedInk.WFC.ModuleSet modules);
```
#### Parameters
<a name='global__WCFConfigObject_TModuleObject_TModule__CreateSpace(BrewedInk_WFC_ModuleSet)_modules'></a>
`modules` [ModuleSet](ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
the modules that have been configured from the Scriptable Object Inspector
  
#### Returns
[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')  
You should return a new GenerationSpace instance that respects the seed properties. 
