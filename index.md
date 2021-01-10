To install gems, you need to authenticate to GitHub Packages by editing the ~/.gemrc file for your project to include https://USERNAME:TOKEN@rubygems.pkg.github.com/OWNER/. You must replace:

USERNAME with your GitHub username.
TOKEN with your personal access token.
OWNER with the name of the user or organization account that owns the repository containing your project.
If you don't have a ~/.gemrc file, create a new ~/.gemrc file using this example.

---
:backtrace: false
:bulk_threshold: 1000
:sources:
- https://rubygems.org/
- https://USERNAME:TOKEN@rubygems.pkg.github.com/OWNER/
:update_sources: true
:verbose: true  
To authenticate with Bundler, configure Bundler to use your personal access token, replacing USERNAME with your GitHub username, TOKEN with your personal access token, and OWNER with the name of the user or organization account that owns the repository containing your project.
