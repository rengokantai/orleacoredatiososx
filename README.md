#### orleacoredatiososx
#####
######3-3
managedObjectModel, persistentStoreCoordinator,managedObjectContext
######12-4 accessing an attribute property list
DetailViewController.swift
```
let context = (UIApplication.sharedApplication().delegate as! AppDelegate).managedObjectContext
let entity = NSEntityDescription.entityForName("Event",inManagedObjectContext:context)
let userInfo = entity?valueForKey("userInfo")
print(userInfo!.valueForKey("abc"))
```
```
let another = entity?.attributesByName["cost"].valueForKey("userInfo")
```
#####13
######13-2Using a fetched resuts controller at runtime
```
let fetchRequestFromTemplate = self.managedObjectModel!.fetchRequestFromTemplateWithName("AllEvents",substitutionVariables:[:])
fetchRequestFromTemplate.sortDescriptors = [sortDsecriptor]
```


