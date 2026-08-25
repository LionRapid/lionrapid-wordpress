# LionRapid Translation — WordPress plugin

Server-side translation for WordPress, powered by the [LionRapid](https://www.lionrapid.com)
translation platform: translated HTML before it reaches the browser, Gutenberg
blocks, a language switcher, `/{lang}/` URL rewriting and hreflang tags.

## Install

1. Download `lionrapid-<version>.zip` from the latest
   [release](https://github.com/LionRapid/lionrapid-wordpress/releases/latest).
2. In WordPress go to **Plugins → Add New → Upload Plugin**, choose the ZIP,
   and activate.
3. Enter your integration key under **Settings → LionRapid**.

The manual is at [docs.lionrapid.com/developers/wordpress-plugin](https://docs.lionrapid.com/developers/wordpress-plugin/).

## Source

This repository holds the plugin's source as released: each release is one
commit on `main`, tagged with its version, with the installable ZIP attached to
the release. Development happens in a private monorepo; releases are published
here automatically.

Bug reports and feature requests: [issues](https://github.com/LionRapid/lionrapid-wordpress/issues).

## License

MIT — see [LICENSE](LICENSE).
