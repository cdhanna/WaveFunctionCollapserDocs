#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WCFConfigObject&lt;TModuleObject,TModule&gt;](WCFConfigObject_TModuleObject_TModule_.md 'BrewedInk.WFC.WCFConfigObject&lt;TModuleObject,TModule&gt;')
## WCFConfigObject&lt;TModuleObject,TModule&gt;.TryGetObject(Module, TModuleObject) Method
Given the typeless Module, get the wrapper object for it. The wrapper object may have additional metadata about the module that isn't used in the WFC algorithm, but may be useful for other parts of the game.  
```csharp
public bool TryGetObject(BrewedInk.WFC.Module module, out TModuleObject moduleObject);
```
#### Parameters
<a name='BrewedInk_WFC_WCFConfigObject_TModuleObject_TModule__TryGetObject(BrewedInk_WFC_Module_TModuleObject)_module'></a>
`module` [Module](Module.md 'BrewedInk.WFC.Module')  
The module you want to get the wrapper object for
  
<a name='BrewedInk_WFC_WCFConfigObject_TModuleObject_TModule__TryGetObject(BrewedInk_WFC_Module_TModuleObject)_moduleObject'></a>
`moduleObject` [TModuleObject](WCFConfigObject_TModuleObject_TModule_.md#BrewedInk_WFC_WCFConfigObject_TModuleObject_TModule__TModuleObject 'BrewedInk.WFC.WCFConfigObject&lt;TModuleObject,TModule&gt;.TModuleObject')  
The wrapper object for the Module. Or null if there is no wrapper object for the given Module
  
#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
True if there was an associated wrapper object with the module, or false.
