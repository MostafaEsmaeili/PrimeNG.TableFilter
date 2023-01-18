# PrimeNG TableFilter to IQueryable Extension

This is a C# extension for the [PrimeNG Table](https://www.primefaces.org/primeng/#/table) that allows for easy conversion of the Table's filter state to an `IQueryable` for use in filtering data in a backend service.



## Usage

To use the extension, simply call the `ToIQueryable` extension method on the `Table` instance, passing in your `IQueryable` data source and a lambda expression for the mapping of the filter state to your data model.

```c#
var filteredData = table.PrimengTableFilter(...);
```
The extension will automatically handle parsing and applying the filter state to the IQueryable, allowing for easy integration with a backend service for filtering large data sets.

Note
This extension is using the DynamicLinq library for generating the filter expression from the filter state of the table.

This package is basically an extension for PrimeNG Table component, it allows you to easily filter data in your backend service by converting the Table's filter state to an IQueryable. It supports usage of lambda expressions for mapping the filter state to your data model and allows to use multiple filterable columns.
