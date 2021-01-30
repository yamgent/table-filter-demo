# table-filter-demo

I originally developed this at https://codesandbox.io/s/table-filter-demo-v6urc,
but now it has its own repo yay.

Features:

- Filter hooks (see `filters/` folder)
  - Filter values are now controllable.
  - Rendering of menu / search dropdown is provided by the hooks.
  - Exposes filter values to support the use case of calling BE
    endpoints when the filter values change.
  - Easy to use - just spread the column props and plug into table
    state hook, done.
- Table state hook (`useTableState`)
  - Management of the filter, sorting and pagination state.
  - Possible to save & restore the last session's table state (NOTE: Doesn't
    work for filters atm, a bit more complex to implement...)
  - Just plug into antd's `<Table />` to use it straightaway.
