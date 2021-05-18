# NiceHash QuickMiner multilanguage support

From [version 0.5.0.0 NiceHash QuickMiner](https://github.com/nicehash/NiceHashQuickMiner/releases) comes with multilanguage support.

### How to create language file?
Download [dump_en.json](/lang/dump_en.json). All strings are marked with token (first element of the array). Modify only second element of the array.

Name your file with two letters - code of the language (eg: en, de, pt, es, ru, ...) plus .json. File format **must be JSON and file encoding must be UTF8!** All language files are located in this directory. Verify your JSON file. There are many tools, for example: https://jsonformatter.curiousconcept.com/

Submit pull request and your translation may gets accepted.

### How to test language file?
Pick any existing language besides **en** and quit NiceHash QuickMiner. Open directory `.\langs\`. You will see language file of the chosen language. Open it and set your language file to have the same `version`. Delete chosen language file, copy in your language file and set your language file to have same name as deleted language. Start NiceHash QuickMiner - selected language will be yours.

Append command line arguments to view special dialogs as stated in the following table:
Command Line | Dialog Shown
-------------|--------------
--install | Download & installer
--uninstall | Uninstall dialog
--count | Windows start-up counter before standard launch
--updatedfrom 0.3.0.0 | Displays various update-related message boxes before standard launch

Example: `NiceHashQuickMiner.exe --install`

To revert this state simply delete your language file.

### How to update language file?

When new strings are added or modified, version gets increased. Using selected language (set it in config file), execute:
`NiceHashQuickMiner.exe --language-dump`

This will dump your language file and make a console printout of missing strings. In production, missing strings are filled with English version of string. When existing strings are modified, it will be noted [here](/lang/UPDATES.md) which strings have been updated.

Again, file must be valid JSON format (verify!) and UTF8 encoded.

When you have all the updates done, submit pull request.


### Special: Translating EULA RTF

> NOTE: Must use latest NiceHashQuickMiner.exe; download: https://github.com/nicehash/NiceHashQuickMiner/releases

Write text in WordPad first, style it and save into any file eg.: _example.rtf_. Then execute:

`NiceHashQuickMiner.exe --port-rtf example.rtf translated.txt`

Your translated and formatted text is ported and ready in file _translated.txt_. Copy it out and put into language file.
