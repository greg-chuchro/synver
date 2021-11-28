# synver
Synver is a versioning system that puts security and reliability above anything else and encourages continuous integration.


|| increment condition | possible implications |
|:-:|:-|:-|
| __MAJOR__ | milestone reached | compilation errors and/or runtime errors |
| __MINOR__ | API declaration change | compilation errors |
| __PATCH__ | API definition change| runtime errors |

## Get Started
```
dotnet tool install --global Ghbvft6.Synver
````
```
synver <NEW_DLL> <OLD_DLL> [VERSION]
```
### Example Output
```
0.1.0

[changed]
Calq.Configuration.Config PrivateScope, Public, Static, HideBySig T Load[T]()
Calq.Configuration.Config PrivateScope, Public, Static, HideBySig System.Void Load[T](T&)

[deleted]
Calq.Configuration.Config PrivateScope, Public, Static, HideBySig System.Void Deserialize[T](System.Text.Json.Utf8JsonReader, T&)

[added]
Calq.Configuration.Attributes.OptionsAttribute None System.Object TypeId
Calq.Configuration.Attributes.OptionsAttribute PrivateScope, Public, Virtual, HideBySig System.Boolean Equals(System.Object)
Calq.Configuration.Attributes.OptionsAttribute PrivateScope, Public, Virtual, HideBySig System.Int32 GetHashCode()
Calq.Configuration.Attributes.OptionsAttribute PrivateScope, Public, Virtual, HideBySig, VtableLayoutMask, SpecialName System.Object get_TypeId()
Calq.Configuration.Attributes.OptionsAttribute PrivateScope, Public, Virtual, HideBySig, VtableLayoutMask System.Boolean Match(System.Object)
Calq.Configuration.Attributes.OptionsAttribute PrivateScope, Public, Virtual, HideBySig, VtableLayoutMask System.Boolean IsDefaultAttribute()
Calq.Configuration.Attributes.OptionsAttribute PrivateScope, Public, HideBySig System.Type GetType()
Calq.Configuration.Attributes.OptionsAttribute PrivateScope, Public, Virtual, HideBySig, VtableLayoutMask System.String ToString()
```
