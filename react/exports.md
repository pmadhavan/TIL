
In JavaScript, especially within the context of React and other modern frameworks, you'll encounter two primary methods for exporting modules (which can be components, functions, constants, etc.): named exports and default exports. Each method has its own use cases, advantages, and disadvantages.

### Named Exports
Named exports allow you to export multiple values from a single module. When importing named exports, you must use the exact name of the exported entity, wrapped in curly braces.

```import { Search } from './Components/Search';```

### Default Exports
A default export allows a module to export a single value as its "default" export. When importing a default export, you can use any name you like for it, and curly braces are not required.

```import { Search } from './Components/Search'; ```

In React, if you are trying to import a componnet into another, you might need to know what type of export is the importing component, and use curly braces based on it, for example, if you try to
import a named exported component without a curly braces, you would see following error

```
Element type is invalid: expected a string (for built-in components) or a class/function (for composite components) but got: undefined.
You likely forgot to export your component from the file it's defined in, or you might have mixed up default and named imports.

Check the render method of `App`.
```
