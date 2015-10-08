AICP Translator Repositories
==========================

The local manifest file needed for AICP's translators.

These local_manifest file are dedicated for branch AICP-lp5.1
------

You need to be in your source folder.

Add TranslationTools repository:
------

If you want to add TranslationTools to help you to find untranslated strings.

    curl https://raw.githubusercontent.com/DelphinPETER/TranslatorRepo/AICP-lp5.1/TranslationTools.xml > .repo/local_manifests/TranslationTools.xml
    repo sync
    
When the sync is finished, you can find TranslationTools under SOURCE_FOLDER/tools/TranslationTools
