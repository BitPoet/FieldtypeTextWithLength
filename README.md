# FieldtypeTextWithLength
Extended FieldtypeText with a subfield selector .length for string length comparison for the ProcessWire CMS/CMF

## Description
This module is just a small extension to FieldtypeText that allows you to search the field's content based on its length.

The search is based on the number of characters, not bytes.

Example:
```php
$pagesWithShortNames = $pages->find('name.length<6');
```

## Usage
Switch any fields you want to be searchable by length from __Text__ to __Text with .length Selector__.

Since FieldtypeTextWithLength extends the regular FieldtypeText, you can switch back and forth between the
two without loosing any data.

After switching a field to this fieldtype, you will also be able to select the Length subfield in Lister
(i.e. in _Pages_ -> _Find_ in the PW backend).

![Example for Lister](https://raw.githubusercontent.com/BitPoet/bitpoet.github.io/master/img/fttwl.png)

## License
Released under Mozilla Public License v2. See file LICENSE for details.
