# WorldEditorRemixTL

The .dll is created with vs2019 using this [tutorial](https://docs.microsoft.com/en-us/cpp/build/creating-a-resource-only-dll).

Future versions of the program could make the previous generated .dll files useless.

### Project design
- Sample/ => EN
- IT/ => IT
- DE/ => DE

We will use different branches for different RC versions, but the same branch for each language.

### Downloadable Translations
Check the [Releases](https://github.com/martysama0134/WorldEditorRemixTL/releases)

### Known Issues
`external symbol not resolved _DllMainCRTStartup`
You're buiding it on x64. You must choose architecture target x86.

`cannot open include file 'afxres.h'`
Renaming it to windows.h inside the .rc file should suffice usually. If not, install MFC and ATL from Visual Studio Installer.
