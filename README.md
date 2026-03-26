# CLaunch Language Modules

## Overview

This repository contains language modules for CLaunch.

You can:
- Update an existing language module
- Create a new language module


## Development Environment

The language project is created for **Microsoft Visual Studio 2026**.  
Visual Studio 2026 can coexist with older versions on the same machine, so installing it will not affect your existing development environments.  
For non-commercial use, the **Visual Studio Community Edition** can be used free of charge.

Download: &nbsp; https://visualstudio.microsoft.com/downloads/


## Updating an existing language

1. Open **CLaunch-Languages.sln** in Visual Studio.
2. Select the **Resource View** tab (usually located in the bottom-left panel).
3. Expand the target language (for example, **Chinese**) in the Resource View.
4. Open each resource (Dialog, Menu, String Table) and edit the text in the resource editor.
5. Build the project if you want to test your changes. See **Build** section below.


## Creating a new language

1. Copy the **English** folder and rename it to your language name.
2. Rename **English.rc** and **English.vcxproj** to your language name.
3. Open the renamed **YourLanguageName.vcxproj** in a text editor and replace **English** with your language name.
4. Open **CLaunch-Languages.sln** in Visual Studio.
5. Select *File* -> *Add* -> *Existing Project...* and add **YourLanguageName.vcxproj**.
6. Select the **Resource View** tab (usually located in the bottom-left panel).
7. Expand **YourLanguageName** and open each resource (Dialog, Menu, String Table) in the Resource View.
8. Edit and translate the text in the resource editor.
9. Build the project if you want to test your changes. See **Build** section below.


## Build

1. Select the build configuration and platform from the toolbar:
   - Configuration: **Release**
   - Platform: **x86** or **x64**

2. From the **Build** menu, choose one of the following:

   - **Build Solution**  
     Builds all language modules included in the solution.

   - **Build (LanguageName)**  
     Builds only the selected language module (the one currently selected in Resource View).

   The output DLL file will be created in the **_output** folder.

## Using a language module

1. Copy the created DLL file to **CLaunch\Languages** folder.
2. Select **Languages...** from the main menu.
3. Choose your language from the list.


## Notes

- **IDS_VERSION** must match the latest version. (Do not change only the number.)

- Do not remove placeholders such as **%d** or **%s**.

- Add your name in the *About* dialog as a translator.  
  You can also set:
  - **IDC_ST_URL_TR** (your website)
  - **IDC_ST_EMAIL_TR** (your email)  
  These can be left blank if not needed.

- If you provide documentation in your language:
  - Place it in the **Docs** folder
  - Update **IDS_DOCUMENT_FILE**


## Translation collaborators

- Simplified Chinese  
  Translated by th_sjy &nbsp; ( http://www.th-sjy.com )

- Traditional Chinese  
  Translated by undecV, SongJim &nbsp; ( https://github.com/undecV/CLaunch_ZH-TW )

- Korean  
  Translated by Miyuki Rose

- Russian  
  Translated by wvxwxvw &nbsp; ( https://github.com/wvxwxvw/translation )

- Spanish  
  Translated by Leonel Mira &nbsp; ( https://github.com/leox23 )

<br/>

------------------------------------------------------------

Author : Pyonkichi  
Website : https://ss1.xrea.com/pyonkichi.g1.xrea.com/en/  
E-mail : pyonky_claunch@yahoo.co.jp

------------------------------------------------------------
