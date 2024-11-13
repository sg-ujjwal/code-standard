## Laravel (PHP)

Refer to the [Mindtwo Laravel Coding Guidelines](https://www.mindtwo.de/guidelines/coding/laravel) for comprehensive guidelines. The following is a summary:

- Naming conventions: Use Use `snake_case` for variable names, `lowerCamelCase` for methods, and `StudlyCase` for classes.
- Indentation: Use 2 spaces for indentation.
- Controller methods: Use RESTful naming conventions for controller methods (e.g., index, create, store, show, edit, update, destroy).
- Validation: Use Laravel's built-in validation rules and create custom rules when necessary.
- Migrations: Name migrations descriptively and keep them in chronological order.

```php
class UserController extends Controller
{
  public function index()
  {
    return User::all();
  }
}
```
## Using the Prettier extension

The [Prettier extension](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) for VS Code can be used to automatically format your code to adhere to the above guidelines. To use it, install the extension and press `F1` or `Ctrl + Shift + P` to open the Command Palette. Then, select `Format Document With...` and choose `Prettier`. A Prettier configuration file is included in the project root directory. This file can be used to configure Prettier to format your code according to the above guidelines automatically.

## Code Comments

Adding comments to your code can help you and others better understand what the code does, how it works, and why certain decisions were made. Here's how to comment various parts of your code using TypeScript and PHP:
```php
/**
 * This function concatenates two strings and returns the concatenated result.
 * @param string $str1 The first string to concatenate
 * @param string $str2 The second string to concatenate
 * @return string The concatenated string
 */
function concatStrings(string $str1, string $str2): string
{
  return $str1 . $str2;
}
```

In this example, a comment block is used to describe the function and its inputs and outputs.


#### PHP:

```php
class Cat
{
  /**
   * Creates a new Cat with the given name and age.
   * @param string $name The name of the cat
   * @param int $age The age of the cat
   */
  public function __construct(string $name, int $age)
  {
    $this->name = $name;
    $this->age = $age;
  }
}
```

In this example, a comment block is used to describe the constructor of the `Cat` class and its inputs.

Adding comments like this to your code can make it much easier to understand and maintain, so be sure to use them in your own projects!

## SCSS

The following is a summary:

- Naming conventions: Use `kebab-case` for class names.
- Indentation: Use 2 spaces for indentation.
- Nesting: Avoid excessive nesting. Keep it to a maximum of 3 levels.
- Variables: Use variables for colors, font sizes, and other reusable values.
- Mixins: Use mixins for reusable styling patterns.
- Media queries: Place media queries near the related styles, not in separate blocks or files.
- All custom components and styling should, if possible, expand from and utilize the [Bootstrap](https://getbootstrap.com/docs/4.6/getting-started/introduction/) library.

```scss
.button {
  background-color: var(--primary-color);
  font-size: var(--base-font-size);
  border-radius: var(--border-radius);

  &:hover {
    background-color: darken(var(--primary-color), 10%);
  }

  @media (max-width: var(--mobile-breakpoint)) {
    font-size: var(--mobile-font-size);
  }
}
```

