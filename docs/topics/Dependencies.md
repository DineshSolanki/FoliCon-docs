# Dependencies

<web-summary>Libraries, services, and runtime requirements that FoliCon depends on.</web-summary>

## System Requirements

| Requirement          | Minimum                                                                                                              |
|----------------------|----------------------------------------------------------------------------------------------------------------------|
| **Operating System** | Windows 10 or Windows 11                                                                                             |
| **.NET Runtime**     | [.NET 10](https://aka.ms/dotnet-download) or higher                                                                  |
| **WebView2 Runtime** | Pre-installed on Windows 11. [Download for older versions](https://developer.microsoft.com/microsoft-edge/webview2/) |

<note>WebView2 Runtime is required for the Overlay Store and other web-based features. It is bundled with Windows 11 and Microsoft Edge.</note>

## External Services

- [The Movie Database (TMDB)](https://www.themoviedb.org/) — Movies and TV show metadata and posters
- [IGDB](https://www.igdb.com/) — Game metadata and artwork (via Twitch API)
- [DeviantArt](https://www.deviantart.com/) — Professional Mode icon browsing and downloads
- [FoliCon-Overlays](https://github.com/DineshSolanki/FoliCon-Overlays) — Community overlay catalog for the Overlay
  Store

## Libraries

- [IconLib](https://github.com/pierresprim/IconLib/pkgs/nuget/WinCopies.IconLib) — Creates `.ico` files from images
- [Handy Controls](https://github.com/ghost1372/HandyControls/) — Custom WPF UI controls
- [Ookii.Dialogs.Wpf](https://github.com/caioproiete/ookii-dialogs-wpf) — File and folder dialogs
- [NLog](https://nlog-project.org/) — Application logging
- [Sentry](https://sentry.io/) — Error tracking and reporting

<tip>

See the full dependency graph on
GitHub: [FoliCon Dependencies](https://github.com/DineshSolanki/FoliCon/network/dependencies)

</tip>
