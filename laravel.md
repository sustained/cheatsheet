# Validation

## Exists

Validating if something exists in the DB is as simple as:

```php
$this->validate($request, ['category_id' => 'exists:categories,id']);
```
# Miscellaneous

## Route-Model Binding

### Binding on something other than the id

You can add a `getRouteKeyName` method to a Model to override the default:

```php
public function getRouteKeyName()
{
    return 'slug';
}
```
