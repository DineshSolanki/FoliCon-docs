# Code Contribution

<web-summary>Learn how to set up the FoliCon development environment and submit a pull request.</web-summary>

Feel free to contribute to the project by opening a pull request. Please make sure to follow the existing code style of the project.

<note>FoliCon requires .NET 10 SDK or higher to build. Download it from <a href="https://aka.ms/dotnet-download">Microsoft's .NET download page</a>.</note>

## General Guidelines

<procedure title="Submit a contribution" id="submit-contribution">
    <step><a href="https://github.com/DineshSolanki/FoliCon/fork">Fork the repository</a> on GitHub.</step>
    <step>Clone your fork: <code>git clone &lt;your-fork-url&gt;</code></step>
    <step>Create a new branch from <code>master</code>: <code>git checkout -b &lt;branch-name&gt;</code></step>
    <step>Make your changes, following the existing code style.</step>
    <step>Commit your changes: <code>git commit -am 'Add some feature'</code></step>
    <step>Push to your branch: <code>git push origin &lt;branch-name&gt;</code></step>
    <step>Submit a pull request against the <code>master</code> branch.</step>
    <step>The CI/CD pipeline will run automated checks on your PR. Wait for them to pass and for the review to complete.</step>
    <step>Celebrate 🎉</step>
</procedure>

<tip>FoliCon uses a CI/CD pipeline that automatically runs tests and publishes releases. Make sure your changes pass all checks before requesting a review.</tip>



<img src="https://media.tenor.com/bI99D4EN9WcAAAAC/merged-pull-request.gif" alt="PR merge celebration gif" border-effect="rounded"/>