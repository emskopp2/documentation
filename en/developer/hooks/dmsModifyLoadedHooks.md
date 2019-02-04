# dmsModifyLoaded... - Hooks

The following hooks could be used for modifying the objects loaded by `DmsLoader`.

**Content**
<!-- toc -->


## dmsModifyLoadedCategory

The "dmsModifyLoadedCategory" hook is triggered for modifying the categories loaded by `DmsLoader`. So the properties could be modified.
It passes the `$category` (existing loaded object) and the `$dbResultCategory` (the database result).
It expects the modified category as return value.

*(since Version 2.2.0)*


```php
// config.php

$GLOBALS['TL_HOOKS']['dmsModifyLoadedCategory'][] = array('MyDmsModificationClass', 'myDmsModifyLoadedCategory');

// MyDmsModificationClass.php

class MyDmsModificationClass
{
	public function myDmsModifyLoadedCategory(\ContaoDMS\Category $category, $dbResultCategory)
	{
		// do custom modification here
		return $category;
	}
}
```


## dmsModifyLoadedAccessRight

The "dmsModifyLoadedAccessRight" hook is triggered for modifying the access rights loaded by `DmsLoader`. So the properties could be modified.
It passes the `$accessRight` (existing loaded object) and the `$dbResultAccessRight` (the database result).
It expects the modified access right as return value.

*(since Version 2.2.0)*


```php
// config.php

$GLOBALS['TL_HOOKS']['dmsModifyLoadedAccessRight'][] = array('MyDmsModificationClass', 'myDmsModifyLoadedAccessRight');

// MyDmsModificationClass.php

class MyDmsModificationClass
{
	public function myDmsModifyLoadedAccessRight(\ContaoDMS\AccessRight $accessRight, $dbResultAccessRight)
	{
		// do custom modification here
		return $accessRight;
	}
}
```


## dmsModifyLoadedDocument

The "dmsModifyLoadedDocument" hook is triggered for modifying the documents loaded by `DmsLoader`. So the properties could be modified.
It passes the `$document` (existing loaded object) and the `$dbResultDocument` (the database result).
It expects the modified access right as return value.

*(since Version 2.2.0)*


```php
// config.php

$GLOBALS['TL_HOOKS']['dmsModifyLoadedDocument'][] = array('MyDmsModificationClass', 'myDmsModifyLoadedDocument');

// MyDmsModificationClass.php

class MyDmsModificationClass
{
	public function myDmsModifyLoadedDocument(\ContaoDMS\Document $document, $dbResultDocument)
	{
		// do custom modification here
		return $document;
	}
}
```
