# "dmsModifyLoaded..."-Hooks

Die folgenden Hooks können verwendet werden um Objekte zu ändern die vom `DmsLoader` geladen wurden.

## dmsModifyLoadedCategory

Der "dmsModifyLoadedCategory"-Hook wird zum Ändern von Kategorien nach dem Laden durch den `DmsLoader` ausgeführt. So können die Eigenschaften verändert werden.
Er übergibt `$category` (vorhandenee geladenes Objekt) und `$dbResultCategory` (das Datenbank-Ergebnis).
Er erwartet die geänderte Kategorie als Rückgabewert.

*(seit Version 2.2.0)*


```php
// config.php

$GLOBALS['TL_HOOKS']['dmsModifyLoadedCategory'][] = array('MyDmsModificationClass', 'myDmsModifyLoadedCategory');

// MyDmsModificationClass.php

class MyDmsModificationClass
{
	public function myDmsModifyLoadedCategory(Category $category, Database_Result $dbResultCategory)
	{
		// do custom modification here
		return $category;
	}
}
```

## dmsModifyLoadedAccessRight

Der "dmsModifyLoadedAccessRight"-Hook wird zum Ändern von Zugriffsrechten nach dem Laden durch den `DmsLoader` ausgeführt. So können die Eigenschaften verändert werden.
Er übergibt `$accessRight` (vorhandenee geladenes Objekt) und `$dbResultAccessRight` (das Datenbank-Ergebnis).
Er erwartet das geänderte Zugriffsrecht als Rückgabewert.

*(seit Version 2.2.0)*


```php
// config.php

$GLOBALS['TL_HOOKS']['dmsModifyLoadedAccessRight'][] = array('MyDmsModificationClass', 'myDmsModifyLoadedAccessRight');

// MyDmsModificationClass.php

class MyDmsModificationClass
{
	public function myDmsModifyLoadedAccessRight(AccessRight $accessRight, Database_Result $dbResultAccessRight)
	{
		// do custom modification here
		return $accessRight;
	}
}
```

## dmsModifyLoadedDocument

Der "dmsModifyLoadedDocument"-Hook wird zum Ändern von Dokumenten nach dem Laden durch den `DmsLoader` ausgeführt. So können die Eigenschaften verändert werden.
Er übergibt `$document` (vorhandenee geladenes Objekt) und `$dbResultDocument` (das Datenbank-Ergebnis).
Er erwartet das geänderte Dokument als Rückgabewert.

*(seit Version 2.2.0)*


```php
// config.php

$GLOBALS['TL_HOOKS']['dmsModifyLoadedDocument'][] = array('MyDmsModificationClass', 'myDmsModifyLoadedDocument');

// MyDmsModificationClass.php

class MyDmsModificationClass
{
	public function myDmsModifyLoadedDocument(Document $document, Database_Result $dbResultDocument)
	{
		// do custom modification here
		return $document;
	}
}
```