### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[Module](./BrewedInk-WFC-Module.md 'BrewedInk.WFC.Module')
## Module.Constraints Field
Every module has a set of [BrewedInk.WFC.ModuleConstraint](https://docs.microsoft.com/en-us/dotnet/api/BrewedInk.WFC.ModuleConstraint 'BrewedInk.WFC.ModuleConstraint'). At the start of the WFC algorithm, every module is possible in all slots.  
The constraints for the module in each slot are all still plausible. As the Wave Function collapses, module possibilities are removed, and various constraints become  
impossible to fulfill. When that happens, this module becomes invalid itself.  
```csharp
public List<ModuleConstraint> Constraints;
```
#### Field Value
[System.Collections.Generic.List](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.List 'System.Collections.Generic.List')  
