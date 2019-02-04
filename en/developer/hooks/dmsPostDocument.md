# dmsPostDocument... - Hooks

The following hooks could be used to execute custom actions after special operations with documents have completed.

**Content**
<!-- toc -->


## dmsPostDocumentDownload

The "dmsPostDocumentDownload" hook is triggered after a documents file has been downloaded. So it is possible to do some custom actions.
It passes the `$strFile` (file name) and the `$document` (existing loaded document with refenrence to category).
It does not expect a return value.

*(since Version 3.0.0)*

```php
// config.php

$GLOBALS['TL_HOOKS']['dmsPostDocumentDownload'][] = array('MyDmsPostDocumentExecutionClass', 'myDmsPostDocumentDownload');

// MyDmsPostDocumentExecutionClass.php

class MyDmsPostDocumentExecutionClass
{
	public function myDmsPostDocumentDownload($strFile, \ContaoDMS\Document $document)
	{
		// do custom actions here
	}
}
```


## dmsPostDocumentUpload

*ToDo*


## dmsPostDocumentEditing

*ToDo*


## dmsPostDocumentDeletion

*ToDo*


## dmsPostDocumentPublishing

*ToDo*
