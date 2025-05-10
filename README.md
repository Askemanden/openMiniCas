# Open Mini Cas


## ENGINE
### casEngine
This is the main engine module, that contains all cas-functionality.

#### Input form
The engine takes input line by line. It stores all values and functions declared on a line

#### Syntax
|functionality|syntax|additional rules|
|-|-|-|
|declare named variable|`name = value`|``name`` cannot start with a number, operator or other reserved symbol or name. The `name` cannot contain reserved symbols, (,),*,/...|
|declare named function|`name(inputVariable1, inputVariable2...)=expression`|`name` must follow variable naming rules. `inputVariable`'s must also follow naming rules|
|redeclare variable or function|`name=values` or `name(inputVariable1...)=expression`|the engine will not prevent reassignments of names|
|call function|`name(param1,param2...)`|function calls must match the number of function inputs.|
|acces variables|`name`|accessing non-existent variables can be done, and will alter any definitions they're used in once they're assigned|