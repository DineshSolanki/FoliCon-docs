# Subfolder processing

<web-summary>
Discover the power of Subfolder Processing, introduced in FoliCon 4.2 and enhanced in v5.2.0. Learn to customize regular expression patterns, control scan depth, skip processed folders, and efficiently manage media in nested folders.
</web-summary>

<show-structure for="chapter,procedure" depth="2"/>

Introduced in version 4.2, FoliCon can search for the media in the nested folders.
You can enable this feature from the settings
and also be able to set regular expression patterns to include or exclude folders.

FoliCon provides 3 default patterns :
<note>Although it's not possible to edit or delete the default patterns, they can definitely be turned on or off.</note>

1. **\S+** - This pattern will include all the folders. (Enabled by default)
2. **Season [0-9]{1,2} Episode [0-9]{1,2}** - This pattern will include folders with the format `Season 01 Episode 01`.
3. **S[0-9]{1,2}E[0-9]**—This pattern will include folders with the format `S01E01`.

You can also add your own patterns and remove or enable/disable as required.

<img src="Subfolder-processing.png" border-effect="rounded" alt="Subfolder processing menu"/>

Configure the patterns as required and click on the save button to add the patterns.
Test the patterns by entering text into the test box after adding the patterns.

Click on the `Enable subfolder processing` checkbox to enable/disable the feature.
If you only want some patterns disabled, you can do that as well.

<note>Subfolder processing can also be toggled while searching</note>

## Processing Options

<img src="subfolder-options-v520.png" border-effect="rounded" alt="Subfolder processing options v5.2.0"/>

### Create icon for root/parent folder

<tldr>
    <ui-path>Settings | Subfolder Processing | Create icon for root/parent folder</ui-path>
    <p>Include or exclude the root folder from icon creation</p>
</tldr>
<p>
When subfolder processing is active, FoliCon can also create an icon for the parent/root folder that was loaded, not just its subfolders. Toggle this option to include or exclude the root folder from icon creation.
</p>

### Subfolder depth limit

<tldr>
    <ui-path>Settings | Subfolder Processing | Subfolder depth limit</ui-path>
    <p>Limit how many levels deep FoliCon searches for media</p>
    <p>Default: unlimited</p>
</tldr>
<p>
Controls how many levels deep FoliCon searches for media. Set a number (e.g., 1 for only immediate subfolders, 2 for two levels deep) to restrict the scan depth. Useful for large libraries where deep folders shouldn't be processed.
</p>

### Skip folders with existing icons

<tldr>
    <ui-path>Settings | Subfolder Processing | Skip folders with existing icons</ui-path>
    <p>Skip any folder that already has a custom icon set</p>
</tldr>
<p>
When enabled, FoliCon skips any folder that already has a custom icon set (i.e., already processed). This is useful for incremental runs where you only want to process newly added folders without overwriting existing icons.
</p>