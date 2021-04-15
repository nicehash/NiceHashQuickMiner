# NiceHash QuickMiner multilanguage support

From version 0.5.0.0 NiceHash QuickMiner comes with multilanguage support.

### How to create language file?
Download [dump_en.json](/lang/dump_en.json). All strings are marked with token (first element of the array). Modify only second element of the array.

Name your file with two letters - code of the language (eg: en, de, pt, es, ru, ...) plus .json. File format **must be JSON and file encoding must be UTF8!** All language files are located in this directory. Verify your JSON file. There are many tools, for example: https://jsonformatter.curiousconcept.com/

Submit pull request and your translation may gets accepted.

### How to update language file?

When new strings are added or modified, version gets increased. Using selected language (set it in config file), execute `NiceHashQuickMiner.exe --language-dump`. This will dump your language file and make a console printout of missing strings. In production, missing strings are filled with English version of string. When existing strings are modified, it will be noted [here](/lang/UPDATES.md) which strings have been updated.

Again, file must be valid JSON format (verify!) and UTF8 encoded.

When you have all the updates done, submit pull request.
