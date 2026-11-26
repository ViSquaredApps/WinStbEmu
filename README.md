# WinStbEmu and FireStb — Public Pages

Public privacy and support website for [WinStbEmu for Windows](https://apps.microsoft.com/detail/9PHJ61Z1D326) and FireStb for Android-based Amazon Fire TV / Fire OS, hosted at `https://visquaredapps.github.io/WinStbEmu/`.

The site source is **ViSquaredApps/WinStbEmu**, not the private application repositories. Keep app source, credentials, signing files, and diagnostic data out of this website repository. Windows and FireStb policies are separate; do not describe the platforms as sharing identical storage, telemetry, billing, or support workflows.

## Pages

| App | Source | Public URL |
|---|---|---|
| WinStbEmu for Windows | `privacy.md` | [Windows Privacy Policy](https://visquaredapps.github.io/WinStbEmu/privacy.html) |
| WinStbEmu for Windows | `support.md` | [Windows Support](https://visquaredapps.github.io/WinStbEmu/support.html) |
| FireStb | `firestb-privacy.md` | [FireStb Privacy Policy](https://visquaredapps.github.io/WinStbEmu/firestb-privacy.html) |
| FireStb | `firestb-support.md` | [FireStb Support](https://visquaredapps.github.io/WinStbEmu/firestb-support.html) |

FireStb uses explicit `.html` permalinks. Internal links use Jekyll's `relative_url` filter so the `/WinStbEmu` base path is retained.

## Build and Deployment

The existing GitHub Pages configuration builds **`main` from the repository root** using Jekyll and the `minima` theme in `_config.yml`. There is no checked-in Gemfile, custom build script, or test suite.

Local drafts do not deploy themselves. After the owner approves the FireStb wording and authorizes publishing, apply the website changes to this repository's `main` branch through the owner's chosen workflow. Leave the private app repositories private; no app repository visibility change is needed for this separate public website.

Before using a FireStb URL in an Amazon listing:

1. Confirm the intended app offer, supported devices, support contact, and actual telemetry/data handling match the submitted build.
2. Resolve any requirement to keep the website source private: this website repository is currently public. Do not change its visibility or publish new content without authorization.
3. Have the owner review applicable privacy obligations, including any retention and data-rights wording; do not invent a retention period, an account-deletion service, or legal guarantees.
4. Publish only after approval, wait for the GitHub Pages build to succeed, and check both FireStb URLs return the correct rendered pages with working links. They are intended URLs until deployment.

With compatible Ruby/Jekyll and the Pages theme dependencies installed, the site can be previewed with `jekyll serve --baseurl /WinStbEmu`. Those tools are not bundled with this repository; inspecting or editing Markdown alone is not a rendered-site build.
