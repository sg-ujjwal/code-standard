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
