#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[Module](Module.md 'BrewedInk.WFC.Module')
## Module.Constraints Field
Every module has a set of [ModuleConstraint](ModuleConstraint.md 'BrewedInk.WFC.ModuleConstraint'). At the start of the WFC algorithm, every module is possible in all slots.  
The constraints for the module in each slot are all still plausible. As the Wave Function collapses, module possibilities are removed, and various constraints become  
impossible to fulfill. When that happens, this module becomes invalid itself.   
```csharp
public List<ModuleConstraint> Constraints;
```
#### Field Value
[System.Collections.Generic.List&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')[ModuleConstraint](ModuleConstraint.md 'BrewedInk.WFC.ModuleConstraint')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List-1 'System.Collections.Generic.List`1')
