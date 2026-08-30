---
switcher-label: IDE
---
# Translations

<web-summary>Contribute translations to FoliCon via Crowdin or directly through the IDE. Learn how to add a new language and submit it to the project.</web-summary>

FoliCon is currently available in the following languages:

1. English
2. Hindi
3. Spanish
4. Arabic
5. Russian
6. Portuguese

FoliCon uses [HandyControls](https://ghost1372.github.io/handycontrol/langs/#Dynamic-Multi-Language) resource files to store strings for each language. They live in the <path>FoliCon/Properties/Langs</path> folder and are named <path>Lang.[language-code].resx</path> — for example, <path>Lang.hi.resx</path> for Hindi.

## Adding a new language via Crowdin {collapsible="true" default-state="expanded"}

[Crowdin](https://crowdin.com/project/folicon) is the recommended way to contribute translations. It gives you a web-based editor, translation memory, and review workflow — no coding environment required.

<tip>Crowdin is the primary and active translation pipeline for FoliCon. New translations and updates are synced automatically into the main repository.</tip>

<procedure title="Contribute via Crowdin" id="crowdin-translate">
    <step>Go to the <a href="https://crowdin.com/project/folicon">FoliCon Crowdin project</a>.</step>
    <step>Sign in or create a free Crowdin account.</step>
    <step>Select your target language and start translating strings in the web editor.</step>
    <step>Submit your translations — they are reviewed and synced into the repository automatically.</step>
</procedure>

## Adding a new language from IDE {switcher-key="Visual Studio" collapsible="true" default-state="collapsed"}

If you prefer to work directly in the source code, you can add a language by creating a resource file in Visual Studio.

1. Right-click on the <path>FoliCon/Properties/Langs</path> folder and select <control>Add > New Item...</control>
   
    <img src="add-new-vs.png" alt="Create Resource file" style="block"/>
2. Select <control>Resource File</control> and name it `Lang.[language-code].resx`

    <img src="add-new-vs.png" alt="Select Resource file" style="block"/>
3. Open the `Lang.resx` file, copy all strings to your new resource file, then translate them.
    
    <img src="lang-vs.png" alt="Copy strings" style="block"/>
4. Open the <path>Languages.cs</path> enum [file](https://github.com/DineshSolanki/FoliCon/blob/master/FoliCon/Models/Enums/Languages.cs) from <path>/Models/Enums/Languages.cs</path> and add the new language to the enum.
   
   <img src="lang-enum-vs.png" alt="Languages enum file"/>
5. Open <path>CultureUtils.cs</path> [file](https://github.com/DineshSolanki/FoliCon/blob/master/FoliCon/Modules/utils/CultureUtils.cs) and add the new language enum and its culture code to the `GetCultureInfoByLanguage` method.
   
    <img src="lang-culture-vs.png" alt="CultureUtils file"/>

## Adding a new language from IDE {switcher-key="Rider" id="adding-a-new-language_1" collapsible="true" default-state="collapsed"}

1. Create a new resource file by either of the following methods:
   1. <control>Right-click</control> on the <path>FoliCon/Properties/Langs</path> folder and select <ui-path>Add > Resources (.resx)</ui-path>
   
        <img src="add-new-rider.png" alt="Create Resource file" style="block"/>
   2. Open any existing resource file, then click <control>Add new culture (+)</control> in the top-right corner, provide a culture tag, and click `Add`.
      
          <img src="add-new-culture-rider.png" alt="Add new culture" style="block"/>
          <img src="add-new-culture-rider-2.png" alt="Add new culture tag" style="block"/>
2. Open any resource file — missing strings for the new language will be highlighted.
3. Add your translations.
4. Open <path>Languages.cs</path> [file](https://github.com/DineshSolanki/FoliCon/blob/master/FoliCon/Models/Enums/Languages.cs) and add the new language to the enum.

   <img src="lang-enum-rider.png" alt="Languages enum file"/>
5. Open <path>CultureUtils.cs</path> [file](https://github.com/DineshSolanki/FoliCon/blob/master/FoliCon/Modules/utils/CultureUtils.cs) and add the new language enum and culture code to the `GetCultureInfoByLanguage` method.

    <img src="lang-culture-rider.png" alt="CultureUtils file"/>

## Testing a new language {collapsible="true" default-state="expanded"}

Build and run FoliCon — the new language should appear in the language dropdown in Settings.

Once verified, submit a pull request to add it to the main repository.

