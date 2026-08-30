# API Keys

<web-summary>Manage API keys for TMDB, IGDB, and DeviantArt in FoliCon.</web-summary>
<show-structure for="chapter,procedure" depth="2"/>

<tldr>
    <ui-path>Menu Bar | Settings | Setup Wizard</ui-path>
    <p>Manage external API credentials for searching and downloading icons.</p>
    <p>Required services: TMDB (movies/shows), IGDB (games), DeviantArt (professional icons).</p>
</tldr>

<p>FoliCon uses three external APIs to fetch metadata, artwork, and icons. You need to provide your own API keys or credentials for these services.</p>

<warning>
Keys are encrypted at rest using DPAPI (Data Protection API) — they never leave your machine.
</warning>

## Setup API Keys

<tabs>
    <tab title="TMDB (Movies & Shows)">
        <p>The Movie Database (TMDB) is used for movies, TV shows, and anime search in Poster Mode.</p>
        <procedure title="How to get a TMDB key" id="tmdb-setup">
            <step>Go to <a href="https://www.themoviedb.org/">themoviedb.org</a> and create a free account.</step>
            <step>Navigate to your profile <strong>Settings</strong>, then open the <strong>API</strong> section.</step>
            <step>Click <strong>Request an API Key</strong> and choose the <strong>Developer</strong> option.</step>
            <step>Fill out the required form details.</step>
            <step>Copy the <strong>API Read Access Token (v4 auth)</strong>.</step>
            <step>In FoliCon, paste the key into the TMDB field of the API Keys settings.</step>
        </procedure>
        <img src="tmdb-api-location.png" border-effect="rounded" alt="TMDB API Read Access Token location"/>
    </tab>
    <tab title="IGDB (Games)">
        <p>The Internet Game Database (IGDB) is used for game search in Poster Mode. It requires a Twitch Developer account.</p>
        <procedure title="How to get IGDB credentials" id="igdb-setup">
            <step>Go to the <a href="https://dev.twitch.tv/console">Twitch Developer Console</a> and log in.</step>
            <step>Click <strong>Register Your Application</strong>.</step>
            <step>Set the OAuth Redirect URL to <code>http://localhost</code>.</step>
            <step>Select <strong>Application Integration</strong> for the Category and submit.</step>
            <step>Copy the <strong>Client ID</strong> and generate/copy the <strong>Client Secret</strong>.</step>
            <step>In FoliCon, paste both the Client ID and Client Secret into the corresponding IGDB fields.</step>
        </procedure>
        <img src="igdb-twitch-console.png" border-effect="rounded" alt="Twitch Developer Console Client ID and Secret"/>
    </tab>
    <tab title="DeviantArt (Icons)">
        <p>DeviantArt is used for Professional Mode browsing and downloading user-created icons.</p>
        <note>DeviantArt is optional — Poster Mode works perfectly fine without it.</note>
        <procedure title="How to get DeviantArt credentials" id="deviantart-setup">
            <step>Go to the <a href="https://www.deviantart.com/developers/">DeviantArt Developers Portal</a>.</step>
            <step>Click <strong>Register Application</strong>.</step>
            <step>Set the OAuth2 Redirect URI to <code>https://localhost</code>.</step>
            <step>Submit the form to get your <strong>Client ID</strong> and <strong>Client Secret</strong>.</step>
            <step>In FoliCon, paste both into the DeviantArt fields.</step>
        </procedure>
        <img src="deviantart-app-credentials.png" border-effect="rounded" alt="DeviantArt Developer Application Credentials"/>
    </tab>
</tabs>

## Managing Keys in FoliCon

<p>You can access the key management panel from <ui-path>Menu Bar | Settings | Setup Wizard</ui-path>. The first-launch wizard also displays this panel to help you get started quickly.</p>

<img src="api-keys-settings.png" border-effect="rounded" alt="API Keys settings in FoliCon"/>

## Troubleshooting

- **Service Unavailable:** If a service shows 'unavailable' after entering a key, double-check for extra spaces when copying the key.
- **Weekly Download Limits:** DeviantArt may show weekly download limit warnings. This is a DeviantArt-side limit on your account, not an issue with your API key.
- **Re-entering Keys:** To update or re-enter a key, open the API Keys panel, clear the field entirely, paste the new key, and save.
