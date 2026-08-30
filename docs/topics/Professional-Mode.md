# Professional Mode

<web-summary>Learn how to find and use high-quality, professionally made folder icons using DeviantArt in Professional Mode.</web-summary>
<show-structure for="chapter,procedure" depth="2"/>

Professional mode is for those who want high-quality professionally made folder icons for their media.

Poster mode initially had Google search as the source for the icons, but it was not reliable,
so it was later changed to use [DeviantArt](https://www.deviantart.com/) [API](https://www.deviantart.com/developers/).

It works very simply, you search for the media, and it shows you the icons, and you can choose from them.

<img src="pro-search-result.png" alt="professional mode search result" />

* See the full preview of any image.
  <img src="pro-full-preview.png" border-effect="rounded" alt="professional mode full preview"/>

<note> Single click on the image to see the full preview</note>
<note> Double click to select the image</note>

[See Extract gallery feature](Extract-gallery.md)

## Watcher-Exclusive Downloads (v5.1.0)

DeviantArt lets creators mark some icon packs as exclusive to their watchers (followers). FoliCon v5.1.0 added the ability to download these watcher-exclusive icons.

To access watcher-exclusive content, you need to authenticate with DeviantArt. There are two ways:
- **OAuth (recommended):** FoliCon guides you through a DeviantArt OAuth login in a browser window. Once authorized, FoliCon can access watcher-exclusive content automatically.
- **Manual credentials:** Enter your DeviantArt Client ID and Client Secret in <ui-path>Menu Bar | Settings | Setup Wizard</ui-path>.

<img src="pro-mode-oauth.png" border-effect="rounded" alt="DeviantArt OAuth login"/>

When browsing in Professional Mode, watcher-exclusive icons show a special badge. If you're authenticated and watching that creator, you can download them just like any other icon.

<img src="pro-mode-watcher-exclusive.png" border-effect="rounded" alt="Watcher-exclusive icons"/>

## DeviantArt Availability and Download Limits

- **Availability:** DeviantArt may occasionally be unreachable due to rate limiting or outages. FoliCon shows a real-time notification in the app when DeviantArt is unavailable. Poster Mode continues to work normally when DeviantArt is down.
- **Weekly download limits (v5.3.0):** DeviantArt has introduced weekly download limits. If you hit the limit, FoliCon shows a clear error message. This mainly affects the Extract Gallery feature. The limit resets weekly on DeviantArt's schedule.

<warning>
If you hit the weekly download limit, you must wait for it to reset on DeviantArt's schedule. FoliCon cannot bypass this limit.
</warning>