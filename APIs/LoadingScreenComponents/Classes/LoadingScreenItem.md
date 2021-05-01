# LoadingScreenItem

### Description

Base class of all LoadingScreen Classes

### Public Override Functions

Name | Description
---- | -----------
[OnProgress](APIs\LoadingScreenComponents\Classes\LoadingScreenItem.md?id=example) | is Called with a progress float assigned with a range from 0 to 1.
[OnReset](APIs\LoadingScreenComponents\Classes\LoadingScreenItem.md?id=example) | is called when the parent [GameObject](https://docs.unity3d.com/500/Documentation/ScriptReference/GameObject.html) with the [LoadingScreenParent](APIs\LoadingScreenComponents\Classes\LoadingScreenParent.md) gets disabled.

### Example

```csharp
public class MyCustomLoadingComponent : LoadingScreenItem
{
    public override void OnProgress(float progress)
    {
        //Set value on Object.
    }

    public override void OnReset()
    {
        //Set original values on Object.
    }
}
```