#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC').[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')
## GenerationSpace.Validate() Method
Evaluate all constraints in the Generation Space and return the number if invalid constraints.  
Ideally, this method should always return zero. However, you can use this to check that the constraints are indeed valid if  
you suspect that the collapse has errored.   
```csharp
public int Validate();
```
#### Returns
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')  
The number of broken constraints in the Generation Space.
