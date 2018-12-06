# Validation

## Exists

Validating if something exists in the DB is as simple as:

```php
$this->validate($request, ['category_id' => 'exists:categories,id']);
```
