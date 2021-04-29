#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## Module Class
In the WFC algorithm, a module is a possibility for some [Slot](Slot.md 'BrewedInk.WFC.Slot')
```csharp
public class Module
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; Module  
### Fields

***
[Constraints](Module_Constraints.md 'BrewedInk.WFC.Module.Constraints')

Every module has a set of [ModuleConstraint](ModuleConstraint.md 'BrewedInk.WFC.ModuleConstraint'). At the start of the WFC algorithm, every module is possible in all slots.  
The constraints for the module in each slot are all still plausible. As the Wave Function collapses, module possibilities are removed, and various constraints become  
impossible to fulfill. When that happens, this module becomes invalid itself.   

***
[Display](Module_Display.md 'BrewedInk.WFC.Module.Display')

Every module must have a unique display name. This name is used for hashing and equality checks.  

***
[Weight](Module_Weight.md 'BrewedInk.WFC.Module.Weight')

A module's weight controls how likely it is to be chosen randomly during a slot collapse. A module with a with a weight of zero will be never be randomly picked.  
