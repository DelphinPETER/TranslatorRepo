Tesla Translator Repositories
==========================

The local manifest file needed for Tesla's translators.

These local_manifest file are dedicated for branch M
------

You need to be in your source folder.

Add TranslationTools repository:
------

If you want to add TranslationTools to help you to find untranslated strings.

    curl https://raw.githubusercontent.com/DelphinPETER/TranslatorRepo/Tesla-M/TranslationTools.xml > .repo/local_manifests/TranslationTools.xml
    repo sync
    
When the sync is finished, you can find TranslationTools under SOURCE_FOLDER/tools/TranslationTools
