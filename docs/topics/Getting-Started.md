# Getting Started

<web-summary>Learn how to download FoliCon, check system requirements, and set up your API keys during the first launch.</web-summary>

<show-structure for="chapter,procedure" depth="2"/>

Welcome to FoliCon! Version 5.0 introduces a Bring Your Own Key (BYOK) system, giving you full control over the services FoliCon uses to fetch metadata and images. 

## System Requirements

Before downloading FoliCon, ensure your system meets the following requirements:

- **Operating System:** Windows 10 or Windows 11
- **.NET Runtime:** .NET 10 or higher. You can download it from [Microsoft's official site](https://aka.ms/dotnet-download).
- **WebView2 Runtime:** Pre-installed on Windows 11. If you are using an older version or it's missing, download it from the [Microsoft Edge Developer site](https://developer.microsoft.com/microsoft-edge/webview2/).

## Download and Install

You can always find the latest release of FoliCon on our GitHub page.

<procedure title="Download FoliCon" id="download-folicon">
    <step>Go to the <a href="https://github.com/DineshSolanki/FoliCon/releases/latest">FoliCon Latest Release</a> page.</step>
    <step>Download the appropriate package for your system.</step>
    <step>Extract the contents to your preferred location and run the executable.</step>
</procedure>

## First Launch Wizard (API Keys)

On your first launch, before reaching the main window, you will be greeted by the onboarding wizard. To use FoliCon, you must set up at least one API key for the services you intend to use.

<note>
Keys are stored securely using DPAPI encryption on your local system. FoliCon never uploads or shares your keys.
</note>

<img src="api-keys-wizard.png" border-effect="rounded" alt="API Keys Wizard window"/>

You only need to configure the keys for the features you actually want to use. If you don't plan on managing games, you can skip the IGDB setup.

### The Movie Database (TMDB)

TMDB provides metadata and images for movies and TV shows.

<procedure title="Get a TMDB API Key" id="tmdb-setup">
    <step>Create a free account at <a href="https://www.themoviedb.org/">TMDB</a>.</step>
    <step>Once logged in, navigate to your <strong>Settings</strong>.</step>
    <step>Go to the <strong>API</strong> section from the left sidebar.</step>
    <step>Follow the instructions to request an API Key.</step>
    <step>Copy the generated API Key into the FoliCon wizard.</step>
</procedure>

### Internet Game Database (IGDB)

IGDB (via Twitch) is used for fetching metadata and artwork for games.

<procedure title="Get IGDB Client ID and Secret" id="igdb-setup">
    <step>Create a <a href="https://dev.twitch.tv/">Twitch Developer</a> account.</step>
    <step>Navigate to your developer console and register a new application.</step>
    <step>Once the app is created, generate a <strong>Client Secret</strong>.</step>
    <step>Copy both the <strong>Client ID</strong> and <strong>Client Secret</strong> into the FoliCon wizard.</step>
</procedure>

### DeviantArt

DeviantArt integration is required if you want to use Professional Mode for finding custom, user-made folder icons.

<procedure title="Get DeviantArt Client ID and Secret" id="deviantart-setup">
    <step>Sign in and go to the <a href="https://www.deviantart.com/developers/">DeviantArt Developers</a> page.</step>
    <step>Register a new application.</step>
    <step>Once registered, locate your application's settings.</step>
    <step>Copy the <strong>Client ID</strong> and <strong>Client Secret</strong> into the FoliCon wizard.</step>
</procedure>

## Updating Your Keys Later

If you skipped a step or need to change a key later, you can easily access the settings from the main application.

<tldr>
    <ui-path>Menu Bar | Settings | API Keys</ui-path>
    <p>Manage and update your service API keys</p>
</tldr>

<tip>
You can also relaunch the entire onboarding wizard from the same settings menu if you prefer a guided experience.
</tip>
