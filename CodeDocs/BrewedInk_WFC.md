## BrewedInk.WFC Namespace
### Classes

***
[AdjacencyConstraint](AdjacencyConstraint.md 'BrewedInk.WFC.AdjacencyConstraint')

A WFC constraint that enforces neighboring modules per slot.  
For example,   
This constraint lets a module express that its western neighbor must be of a certain module.   

***
[GenerationSpace](GenerationSpace.md 'BrewedInk.WFC.GenerationSpace')

The Generation Space is the main access point for the WFC algorithm. The Generation Space holds a directed graph of Slots, and a set of all possible modules per slot.  
The Generation Space has methods for collapsing the superposition of the Slots, until all slots only have one module option left.  

***
[Module](Module.md 'BrewedInk.WFC.Module')

In the WFC algorithm, a module is a possibility for some [Slot](Slot.md 'BrewedInk.WFC.Slot')

***
[ModuleConstraint](ModuleConstraint.md 'BrewedInk.WFC.ModuleConstraint')

The base type for all WFC constraints. Feel free to subclass this type and make your own constraints.   

***
[ModuleSet](ModuleSet.md 'BrewedInk.WFC.ModuleSet')

A ModuleSet is a collection of modules. It is a HashSet, with a few helpful methods attached to it.   

***
[Slot](Slot.md 'BrewedInk.WFC.Slot')

In the WFC algorithm, a Slot is a place that holds one [Module](Module.md 'BrewedInk.WFC.Module'). As the Wave Function is being collapsed, the slot may have many potential modules available to it.  
As the collapse continues, modules are removed as possibilities from the slot, until there is only one module possible for the slot.  
  

***
[SlotCannotHaveEmptyModuleSetException](SlotCannotHaveEmptyModuleSetException.md 'BrewedInk.WFC.SlotCannotHaveEmptyModuleSetException')

An exception that is thrown when the WFC tries to remove the last remaining module from a slot's possibility space. A slot cannot have zero possibilities.  

***
[SlotCannotSelectUnavailableModule](SlotCannotSelectUnavailableModule.md 'BrewedInk.WFC.SlotCannotSelectUnavailableModule')

An exception that is thrown if a slot tries to select a module that is no longer possible, due to constraints.  

***
[SlotEdge](SlotEdge.md 'BrewedInk.WFC.SlotEdge')

A SlotEdge is the connection between two slots. In a simple 2D 1X2 grid case, there are two slots, and one slot edge connecting them.  
The term "edge" comes from Graph Theory. These edges are directional.  

***
[SlotModuleRemoved](SlotModuleRemoved.md 'BrewedInk.WFC.SlotModuleRemoved')

A progress instance that explains what module was removed from a slot's possibility space.  

***
[SlotModuleSelected](SlotModuleSelected.md 'BrewedInk.WFC.SlotModuleSelected')

A progress instance that explains what module was selected for a slot. When this progress type shows up, it means the superposition for the given slot has collapsed to the given module.  

***
[WFCError](WFCError.md 'BrewedInk.WFC.WFCError')

A WFCError instance could be returned by the WFC algorithm. If you receive one of these instances, it means something with the process has broken.  

***
[WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')

The [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress') class represents a unit of progress in the WFC algorithm. As the algorithm is run, a sequence of WCFProgress items will be returned.  
Different types of progress will be returned, and you can switch on the type to gain insights to the algorithm's decisions...  
  

***
[WFCProgressExtensions](WFCProgressExtensions.md 'BrewedInk.WFC.WFCProgressExtensions')

A Utility class for IEnumerable sets of [WFCProgress](WFCProgress.md 'BrewedInk.WFC.WFCProgress')
