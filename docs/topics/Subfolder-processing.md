# Subfolder processing

<web-summary>
Discover the power of Subfolder Processing, introduced in FoliCon 4.2. Learn to customize regular expression patterns to efficiently manage media in nested folders. Explore features allowing enabling, disabling, or adding your own patterns.
</web-summary>


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