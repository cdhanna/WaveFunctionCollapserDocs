#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.GetEntropy(ModuleSet) Method
Calculates the entropy of a set of modules.  
Entropy is ```csharp
 -sum(p log(p) )```
 over all modules where each p is the probability of the module  
```csharp
public float GetEntropy(BrewedInk.WFC.ModuleSet modules);
```
#### Parameters
<a name='BrewedInk_WFC_GenerationSpace_GetEntropy(BrewedInk_WFC_ModuleSet)_modules'></a>
`modules` [ModuleSet](ModuleSet.md 'BrewedInk.WFC.ModuleSet')  
A set of modules
  
#### Returns
[System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single')  
The entropy of the given set of modules
