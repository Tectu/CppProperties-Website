---
weight: 3
bookCollapseSection: true
---

# Properties
Properties are what this library is all about. There are a number of property types available to ensure maximum flexiblity.

To use properties, the client class needs to inherit from `properties` provided by this library:

```cpp
class shape :
	tct::cppproperties::properties
{
	MAKE_PROPERTY(x, int);
	MAKE_PROPERTY(y, int);
}
```

{{< hint info >}}
Note that a property type needs to be registered before it can be used. See [types](../types/_index.md) for more information.
{{< /hint >}}

The following types of properties are available:
- **[Raw properties](./raw_properties.md)**: This is the most common form of a property. Use this if you want to use a regular member variable as a property.
- **[Linked properties](./linked_properties.md)**: Linked properties are used when public or protected member variables of a base class should become properties.
- **[Linked property functions](./linked_property_functions.md)**: Allows to use private members variables of a base class as properties.
