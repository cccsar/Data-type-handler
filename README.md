# Data-type-handler

Data type simulator for atomic types, registers and unions.

This is an interactive program. Instructions follow: 

* `ATOMICO <name> <representation> <alignment>`: Defines a new atomic type of name `<name>` , whose representation takes `<representation>` bytes and must align at `<alignment>` bytes.
* `STRUCT <name> [<type>]`: Defines a new record of name `<name>`. Records fields are described within `[<type>]`. Notice fields won't be named but only described by their type. 
* `UNION <name> [<type>]`: Defines a new union type of name `<name>`. Each variant is described within `[<type>]`. Notice fields won't be named but only described by their type. 
* `DESCRIBIR <name>`: Display information related to type named `<name>`. This information includes size, alignment and wasted bytes for the type if for the following cases:
  - Registers and unions are saved without packaging.
  - Registers and unions are packed.
  - Registers and unions are reordered for optimal storage.
  
## Instrucciones de ejecucion

For IO testing  run `cabal run` and then interact with main program
