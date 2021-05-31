# unity-generic-singleton
Unity Monobehavior Generic Singleton that I'm using in my own projects

# Usage
Add the script into your Unity project and when you need to create Singleton simply use

``` c#
using UnityEngine;

public class YourClassName : GenericSingleton<YourClassName>
{

  protected override void InternalInit()
  {
    //your initiaizaton code
  }
  
    protected override void InternalOnDestroy()
  {
    //your code that will run when object will be destroyed
  }
  
}
```
Morover your Singleton object will have 2 more options that can be changed in the inspector. The atribtes that can be changed are `_deactivateOnLoad` (deactivates GameObject on init) and `_dontDestroyOnLoad` (Not let Unity destroy the GameObject on new scene loaded).

# Disclamer
This code isn't written by me. I add some changes to original one (mostly comments and readability). But I lost the original source. If you are an autor of this code then sorry :)
