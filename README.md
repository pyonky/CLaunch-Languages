# CLaunch Language Modules

## Overview

You can create a CLaunch language module for your language.

## Development Environment

The language project is created for **Microsoft Visual Studio 2026**.  
Visual Studio 2026 can coexist with older versions on the same machine, so installing it will not affect your existing development environments.  
For non-commercial use, the **Visual Studio Community Edition** can be used free of charge.

Download: &nbsp; https://visualstudio.microsoft.com/downloads/

## How to create

1. Copy the *English* folder and change the folder name to your language name.
2. Rename the *English.rc* and *English.vcxproj* files in the copied folder to your language name.
3. Open **YourLanguageName.vcxproj** in a text editor and replace the word *English* with your language name.
4. Open *CLaunch-Languages.sln* with the Visual Studio.
5. Select *File* -> *Add* -> *Existing Project* from the menu and select **YourLanguageName.vcxproj** in the copied folder.
6. Translate the **YourLanguageName.rc** into your language.
7. Select the *Configuration* to *Release*, select the *Platform* to *x86* or *x64* and build.
8. **YourLanguageName.dll** will be created under *_output* folder (Win32 or x64).

## How to use

- Copy the created DLL file to "CLaunch\Languages" folder and select "Languages..." from main menu. Your language name will appear on the "Choose language" dialog box.

## Notes

- IDS_VERSION must be changed to latest version number. (Don't change only version number.)

- Don't remove the placeholders like "%d" and "%s".

- Put your name into lower group box of the *About* dialog box as a translator.
Also IDC_ST_URL_TR should be modified to URL of your website, and IDC_ST_EMAIL_TR should be your e-mail address. But if you don't have a website or you don't want to receive the e-mail, they can be blank or removed.

- if you make the document in your language, put the document file to the Docs folder and modify the IDS_DOCUMENT_FILE to the document file name.

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
