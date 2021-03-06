[com.github.salomonbrys.kodein](../index.md) / [CProvider](.)

# CProvider

`class CProvider<out T : Any> : `[`Provider`](../-provider/index.md)`<T>`

Concrete provider: each time an instance is needed, the function [creator](creator.md) function will be called.

A provider is like a [CFactory](../-c-factory/index.md), but without argument.

### Parameters

`T` - The created type.

`createdType` - The type of objects created by this provider, *used for debug print only*.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `CProvider(createdType: `[`Type`](http://docs.oracle.com/javase/6/docs/api/java/lang/reflect/Type.html)`, creator: `[`ProviderKodein`](../-provider-kodein/index.md)`.() -> T)`<br>Concrete provider: each time an instance is needed, the function [creator](-init-.md#com.github.salomonbrys.kodein.CProvider$<init>(java.lang.reflect.Type, kotlin.Function1((com.github.salomonbrys.kodein.ProviderKodein, com.github.salomonbrys.kodein.CProvider.T)))/creator) function will be called. |

### Properties

| Name | Summary |
|---|---|
| [createdType](created-type.md) | `val createdType: `[`Type`](http://docs.oracle.com/javase/6/docs/api/java/lang/reflect/Type.html)<br>The type of object that is created by this factory. |
| [creator](creator.md) | `val creator: `[`ProviderKodein`](../-provider-kodein/index.md)`.() -> T`<br>The function that will be called each time an instance is requested. Should create a new instance. |

### Inherited Properties

| Name | Summary |
|---|---|
| [argType](../-provider/arg-type.md) | `open val argType: `[`Type`](http://docs.oracle.com/javase/6/docs/api/java/lang/reflect/Type.html)<br>The type of the argument this factory will function for. |
| [description](../-provider/description.md) | `open val description: String`<br>The description of this factory (using simple type names), *used for debug print only*. |
| [fullDescription](../-provider/full-description.md) | `open val fullDescription: String`<br>The description of this factory (using full type names), *used for debug print only*. |

### Functions

| Name | Summary |
|---|---|
| [factoryName](factory-name.md) | `fun factoryName(): String`<br>The name of this factory, *used for debug print only*. |
| [getInstance](get-instance.md) | `fun getInstance(kodein: `[`ProviderKodein`](../-provider-kodein/index.md)`, key: `[`Key`](../-kodein/-key/index.md)`): T`<br>Get an instance of type `T`. |

### Inherited Functions

| Name | Summary |
|---|---|
| [getInstance](../-provider/get-instance.md) | `open fun getInstance(kodein: `[`FactoryKodein`](../-factory-kodein/index.md)`, key: `[`Key`](../-kodein/-key/index.md)`, arg: Unit): T`<br>Get an instance of type `T`. |
