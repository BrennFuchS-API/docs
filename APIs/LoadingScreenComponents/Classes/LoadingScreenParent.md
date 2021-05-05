# LoadingScreenParent

### Description

Parent of any Loading Screen

### Variables:

Name | Description | Type
---- | ----------- | ----
[loadingScreenItems](APIs\LoadingScreenComponents\Classes\LoadingScreenParent.md) | holds the loadingScreen behaviours | [List](https://docs.microsoft.com/de-de/dotnet/api/system.collections.generic.list-1?view=netframework-3.5)<[LoadingScreenItem](APIs\LoadingScreenComponents\Classes\LoadingScreenItem.md)>

### Public Methods:

Name | Description
---- | -----------
[SetProgress](APIs\LoadingScreenComponents\Classes\LoadingScreenParent.md) | Sets the progress (Range 0 to 1) for all children of the LoadingScreenParent with a LoadingScreenItem Component

### Example
```csharp
using UnityEngine;
using LoadingScreenComponents;

YourClass : Monobehaviour
{
    public LoadingScreenParent yourLoadingScreenParent;

    private void Start()
    {
        yourLoadingParent.SetProgress(0.5f); //sets progress to half.
    }
}
```