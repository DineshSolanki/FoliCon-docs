# How to contribute

<web-summary>Learn the different ways you can contribute to FoliCon — code, documentation, translations, bug reports, and custom overlays.</web-summary>

FoliCon is an open-source project, and we welcome contributions from the community.
This guide explains how to contribute to FoliCon.

FoliCon has a lot of potential, and for that, **we need your help**.

## Before you start {collapsible="true"}

FoliCon is written in C# and uses WPF for the UI.

> See the [Dependencies](Dependencies.md) page for more information about the libraries
>
{style="tip"}

Before building FoliCon, you'll need API keys for the services it uses:

- [A TMDB API key](https://www.themoviedb.org/settings/api)
- [An IGDB API (via Twitch)](https://api.igdb.com/)
- [A DeviantArt API key](https://www.deviantart.com/developers/register)

<tip>On first launch, FoliCon guides you through entering these keys via the onboarding wizard. You can also create <path>AppConfig.json</path> manually in the <path>FoliCon</path> folder with the structure below.</tip>

```json
{
  "DevClientID": "Your_DeviantArt_Client_ID_here",
  "DevClientSecret": "Your_DeviantArt_Client_Secret_here",
  "TMDBKey": "Your_TMDB_API_here",
  "IgdbClientId": "Your_IGDB_Client_ID_here",
  "IgdbClientSecret": "Your_Client_Secret_API_here"
}
```

## Ways to contribute

- [Report a bug](https://github.com/DineshSolanki/FoliCon/issues/new/choose)
- [Fix an open bug](https://github.com/DineshSolanki/FoliCon/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc)
- [Code contribution or feature addition](Code-Contribution.md)
- [](Improve-Documentation.md)
- [Add new translations or improve existing ones](Translations.md)
- [Create and share a custom overlay](Creating-an-Overlay.md) — build a new icon overlay style and publish it to the community store

## Discussion for feature requests and bugs

FoliCon uses GitHub issues to track bugs and feature requests.

Please search the existing issues before filing new issues to avoid duplicates.
FoliCon feature discussions are done on the [Discussions](https://github.com/DineshSolanki/FoliCon/discussions/142) page.
