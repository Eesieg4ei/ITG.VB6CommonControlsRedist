Microsoft Visual Basic 6.0 Common Controls Redistributable
==========================================================

MSI пакет для распространения через GPO ActiveX компонентов Visual Basic 6.0, в частности:

- mscomctl.ocx
- mscomct2.ocx

Развёртывание пакета через GPO
------------------------------

Подготовленная административная точка установки расположена в подкаталоге [VB6CommonControlsRedist/bin/Release](../../VB6CommonControlsRedist/bin/Release).
Дополнительной подготовки файла `VB6CommonControlsRedist.msi` через `msiexec -a VB6CommonControlsRedist.msi` не требуется.
Скачайте целиком папку [VB6CommonControlsRedist/bin/Release](../../VB6CommonControlsRedist/bin/Release), разместите на сетевом ресурсе, и - разверните через GPO.

Сборка .msi пакета
------------------

Для внесения изменений в пакет и повторной сборки пакета потребуются следующие продукты:

- Microsoft Visual Studio 2012 Shell:
	-[Isolated](http://www.microsoft.com/ru-ru/download/details.aspx?id=30670)
	-[Integrated](http://www.microsoft.com/ru-ru/download/details.aspx?id=30663)
- [Windows Installer XML Toolset - WIX](http://wixtoolset.org/)

Установить необходимо все пакеты в указанном порядке. В результате - получае MS Visual Studio 2012 с подготовленными
шаблонами проектов WiX. После этого открываем файл решения `VB6CommonControlsRedist.sln` и собираем решение.

Дополнительные сведения
-----------------------

- [достаточно богатая на примеры статья по использованию WiX](http://habrahabr.ru/post/68616/)
