# LoadingScreenItem

### Description

Base class of all LoadingScreen Classes

### Classes based on this one:

Class | Description
----- | -----------
[LoadingBar](APIs\LoadingScreenComponents\Classes\LoadingBar.md) | the classic loading Bar we all know and love.
[LoadingSpinner](APIs\LoadingScreenComponents\Classes\LoadingSpinner.md) | spins an object around a set axis while loading.
[LoadingText](APIs\LoadingScreenComponents\Classes\LoadingText.md) | the classic text showing the progress of the loading.

### Public Override Methods:

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