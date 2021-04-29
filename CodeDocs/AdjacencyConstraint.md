#### [brewkedink.wfc](index.md 'index')
### [BrewedInk.WFC](BrewedInk_WFC.md 'BrewedInk.WFC')
## AdjacencyConstraint Class
A WFC constraint that enforces neighboring modules per slot.  
For example,   
This constraint lets a module express that its western neighbor must be of a certain module.   
```csharp
public class AdjacencyConstraint : BrewedInk.WFC.ModuleConstraint
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [ModuleConstraint](ModuleConstraint.md 'BrewedInk.WFC.ModuleConstraint') &#129106; AdjacencyConstraint  
### Fields

***
[Delta](AdjacencyConstraint_Delta.md 'BrewedInk.WFC.AdjacencyConstraint.Delta')

The positional difference this constraint applies for. If the module is being tested between two slots (A, and B), the constraint only applies if the positional difference between A and B equals the Delta.    

***
[NeedsOneOf](AdjacencyConstraint_NeedsOneOf.md 'BrewedInk.WFC.AdjacencyConstraint.NeedsOneOf')

A set of possible module values that can exist at a slot with the given Delta.   
