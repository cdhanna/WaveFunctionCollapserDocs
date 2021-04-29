#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[WCFConfigObject](WCFConfigObject.md 'BrewedInk.WFC.WCFConfigObject')
## WCFConfigObject.TryGetSprite(Module, Sprite) Method
If a module has a Sprite associated with it, you can use this method to try and get it. Depending on the type of Module, there may not be any Sprite available.   
```csharp
public abstract bool TryGetSprite(BrewedInk.WFC.Module module, out UnityEngine.Sprite sprite);
```
#### Parameters
<a name='BrewedInk_WFC_WCFConfigObject_TryGetSprite(BrewedInk_WFC_Module_UnityEngine_Sprite)_module'></a>
`module` [Module](Module.md 'BrewedInk.WFC.Module')  
The module you'd like to get a sprite for.
  
<a name='BrewedInk_WFC_WCFConfigObject_TryGetSprite(BrewedInk_WFC_Module_UnityEngine_Sprite)_sprite'></a>
`sprite` [UnityEngine.Sprite](https://docs.microsoft.com/en-us/dotnet/api/UnityEngine.Sprite 'UnityEngine.Sprite')  
The Sprite associated with the given module. The sprite will be null if there is no associated Sprite for the module.
  
#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
True if there is any sprite associated with the module, false otherwise. If the method returns false, you can expect the sprite to be null.
