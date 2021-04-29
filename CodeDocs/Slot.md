#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## Slot Class
In the WFC algorithm, a Slot is a place that holds one [Module](Module.md 'BrewedInk.WFC.Module'). As the Wave Function is being collapsed, the slot may have many potential modules available to it.  
As the collapse continues, modules are removed as possibilities from the slot, until there is only one module possible for the slot.  
  
```csharp
public class Slot
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; Slot  
### Fields

***
[Coordinate](Slot_Coordinate.md 'BrewedInk.WFC.Slot.Coordinate')

The slot's position in the larger generation space.   
