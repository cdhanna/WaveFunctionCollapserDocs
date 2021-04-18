### [BrewedInk.WFC](./BrewedInk-WFC.md 'BrewedInk.WFC').[GenerationSpace](./BrewedInk-WFC-GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.TryGetOnlyOption(BrewedInk.WFC.Slot, BrewedInk.WFC.Module) Method
At any given moment, a slot may have many possible modules available to it. However, eventually, a slot will only have one possible module remaining.  
This method will help you identify when there is only one module left per slot.  
If there is only one module left for the given slot, this method will return true and store the assigned module in the out parameter. If there is more than one module possible, the method will return false, and the out variable will be null.  
 
You can also retrieve all of the available slot modules with the ` GenerationSpace.GetSlotOptions ` method.  
[GetSlotOptions(BrewedInk.WFC.Slot)](./BrewedInk-WFC-GenerationSpace-GetSlotOptions(BrewedInk-WFC-Slot).md 'BrewedInk.WFC.GenerationSpace.GetSlotOptions(BrewedInk.WFC.Slot)')  
```csharp
public bool TryGetOnlyOption(BrewedInk.WFC.Slot slot, out BrewedInk.WFC.Module module);
```
#### Parameters
<a name='BrewedInk-WFC-GenerationSpace-TryGetOnlyOption(BrewedInk-WFC-Slot_BrewedInk-WFC-Module)-slot'></a>
`slot` [Slot](./BrewedInk-WFC-Slot.md 'BrewedInk.WFC.Slot')  
The slot whose only remaining available module will be checked.  
  
<a name='BrewedInk-WFC-GenerationSpace-TryGetOnlyOption(BrewedInk-WFC-Slot_BrewedInk-WFC-Module)-module'></a>
`module` [Module](./BrewedInk-WFC-Module.md 'BrewedInk.WFC.Module')  
An out variable for the only remaining available module. After the method is invoked, the value of the module will be the last module for the slot, or null if there are more than one modules remaining.  
  
#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
true if there was only one module available, or false otherwise.  
