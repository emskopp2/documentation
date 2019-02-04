# "dmsModifyLoaded..." - Hooks

Die folgenden Hooks können verwendet werden um Objekte zu ändern die vom `DmsLoader` geladen wurden.

**Inhalt**
<!-- toc -->


## "dmsModifyLoadedCategory" - Hook

Der "dmsModifyLoadedCategory" - Hook wird zum Ändern von Kategorien nach dem Laden durch den `DmsLoader` ausgeführt. So können die Eigenschaften verändert werden.
Er übergibt `$category` (vorhandenes geladenes Objekt) und `$dbResultCategory` (das Datenbank-Ergebnis).
Er erwartet die geänderte Kategorie als Rückgabewert.

*(seit Version 2.2.0)*


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


## "dmsModifyLoadedAccessRight" - Hook

Der "dmsModifyLoadedAccessRight" - Hook wird zum Ändern von Zugriffsrechten nach dem Laden durch den `DmsLoader` ausgeführt. So können die Eigenschaften verändert werden.
Er übergibt `$accessRight` (vorhandenes geladenes Objekt) und `$dbResultAccessRight` (das Datenbank-Ergebnis).
Er erwartet das geänderte Zugriffsrecht als Rückgabewert.

*(seit Version 2.2.0)*


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


## "dmsModifyLoadedDocument" - Hook

Der "dmsModifyLoadedDocument" - Hook wird zum Ändern von Dokumenten nach dem Laden durch den `DmsLoader` ausgeführt. So können die Eigenschaften verändert werden.
Er übergibt `$document` (vorhandenes geladenes Objekt) und `$dbResultDocument` (das Datenbank-Ergebnis).
Er erwartet das geänderte Dokument als Rückgabewert.

*(seit Version 2.2.0)*


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