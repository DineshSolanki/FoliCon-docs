# Creating an Overlay

<web-summary>Learn how to create and publish your own custom overlay packages for FoliCon using the built-in designer or manually.</web-summary>

<show-structure for="chapter,procedure" depth="2"/>

FoliCon v5.3.0 introduced a data-driven overlay package system. Overlays are no longer hardcoded into the app — they are small, distributable packages that FoliCon loads dynamically. Anyone can create one and share it with the community.

## Choose Your Method

There are two ways to build a custom overlay:

<tabs>
<tab title="Overlay Designer (Recommended)">

The [Overlay Designer](Overlay-Designer.md) is the easiest way to get started. It gives you a live WYSIWYG canvas inside FoliCon — no files to write by hand.

1. Open the designer from <ui-path>Poster Icon Config | Open Overlay Designer…</ui-path>
2. Design your overlay visually — adjust layout, text, colours, and positioning
3. Use the live preview to see the result on a real folder icon
4. When you're happy, export it as an overlay package ready to submit

<tip>This is the recommended path for first-time overlay creators.</tip>

</tab>
<tab title="Manual Creation (Advanced)">

If you prefer full control, you can author the overlay package files directly.

An overlay package is a folder that contains three things:

- A `manifest.json` describing the overlay
- An overlay definition file (e.g. `overlay.json`) that defines the visual layout
- A preview image (`preview.png`, 256×256 px or larger)

**Package structure:**

```
MyOverlay/
  manifest.json
  overlay.json
  preview.png
```

<img src="overlay-package-structure.png" border-effect="rounded" alt="Example overlay package structure and preview image"/>

**`manifest.json` fields:**


| Field | Type | Description |
|-------|------|-------------|
| `name` | string | Display name shown in the store |
| `author` | string | Your name or handle |
| `version` | string | Semver version, e.g. `"1.0.0"` |
| `description` | string | Short description shown in the store |
| `tags` | array | Search tags, e.g. `["dark", "minimal", "anime"]` |
| `category` | string | One of: `General`, `Anime`, `Games`, `Movies`, `TV`, `Music`, `Minimal`, `Colorful` |
| `preview` | string | Filename of the preview image, e.g. `"preview.png"` |

<note>Make sure all required fields are present and your JSON is valid before submitting.</note>

</tab>
</tabs>

## Submit to the Community Store

Once your overlay package is ready, you can share it with everyone through the [FoliCon-Overlays](https://github.com/DineshSolanki/FoliCon-Overlays) repository. After it is merged, it appears automatically in the [Overlay Store](Overlay-Store.md) for all FoliCon users.

<procedure title="Submit your overlay" id="submit-overlay">
    <step>Fork the <a href="https://github.com/DineshSolanki/FoliCon-Overlays">FoliCon-Overlays</a> repository on GitHub.</step>
    <step>Add your overlay package folder into the <path>overlays/</path> directory of your fork.</step>
    <step>Open a pull request with a title and description explaining your overlay — what it looks like and what media type it suits best.</step>
    <step>After review and merge, your overlay appears in the Overlay Store automatically. No app update needed.</step>
</procedure>

## Tips for a Great Overlay

- **Use a strong preview image.** The preview is the first thing people see in the store — make it clear and representative of the overlay at its best.
- **Keep the name short and memorable.** Names like `"Minimal Dark"` or `"Doraemon"` work better than long descriptions.
- **Test on both light and dark folder backgrounds** before submitting — some overlays look great on one but not the other.
- **Add meaningful tags.** Good tags help users find your overlay when searching. Think about the media type, visual style, and mood.
- **Bump the version** in `manifest.json` when you update an overlay so existing installs can detect the update.
