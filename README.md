CyanogenMod Translator Repositories
==========================

All local manifest files needed for CyanogenMod's translators.

Those local_manifest files are dedicated for branch cm-11.0
------

You need to be in your source folder.

Add TranslationTools repository:
------

If you want to add TranslationTools to help you to find untranslated strings.

    curl https://raw.githubusercontent.com/DelphinPETER/TranslatorRepo/cm-11.0/TranslationTools.xml > .repo/local_manifests/TranslationTools.xml
    repo sync
    
When the sync is finished, you can find TranslationTools under SOURCE_FOLDER/tools/TranslationTools


Add extra packages repositories:
------

If you want to get all the available CyanogenMod translatable packages that are not synced by default (not included in the default CM manifest), execute:

    curl https://raw.githubusercontent.com/DelphinPETER/TranslatorRepo/cm-11.0/extra_packages.xml > .repo/local_manifests/extra_packages.xml
    repo sync

Hint: if you are already downloaded some device repositories with "breakfast" and have problems syncing, execute:

    rm .repo/local_manifests/roomservice.xml
    repo sync
    breakfast <device>


Add websites repositories:
------

If you want to add get-cm and CMAccountwebsite.

    curl https://raw.githubusercontent.com/DelphinPETER/TranslatorRepo/cm-11.0/cyanogenmod_website.xml > .repo/local_manifests/cyanogenmod_website.xml
    repo sync
    
When the sync is finished, you can find the websites under SOURCE_FOLDER/website/

Remove untranslatable repositories:
------

If you build NEVER NEVER NEVER NEVER CyanogenMod, you could limited the source folder to the translatable projects

Advantages :

1- The source folder will be limited under 4 Go (All the source folder can be upper 27Go)

2- You will limit the downloaded files when you sync



    curl https://raw.githubusercontent.com/DelphinPETER/TranslatorRepo/cm-11.0/untranslatable_project.xml > .repo/local_manifests/untranslatable_project.xml
    repo sync
    
    
