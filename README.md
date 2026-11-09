# Lionrapid Translation for WordPress

Translates your WordPress site on the server, before the page reaches the browser. Every language gets its own
address (`/fi/…`), with the right `lang` attribute, hreflang links and translated titles and descriptions, so search
engines index each language. Translations come from your [Lionrapid](https://www.lionrapid.com) project: machine
translation drafts them, and a person marks them ready before they go live.

- **Plugin directory:** https://wordpress.org/plugins/lionrapid-translation/
- **Product page:** https://www.lionrapid.com/integrations/wordpress
- **Manual:** https://docs.lionrapid.com/developers/wordpress-plugin/

## Requirements

- WordPress 6.0 or newer, PHP 8.1 or newer.
- A Lionrapid account and project. The plugin translates through the Lionrapid service.

## Install

**From the WordPress plugin directory (recommended).** In wp-admin, go to **Plugins → Add New Plugin**, search for
**Lionrapid**, click **Install Now** on Lionrapid Translation, then **Activate**. Updates arrive in
**Dashboard → Updates** like any other plugin's.

**From a ZIP.** Download `lionrapid-translation-<version>.zip` from the
[latest release](https://github.com/LionRapid/lionrapid-wordpress/releases/latest) and upload it under
**Plugins → Add New Plugin → Upload Plugin**. It installs into the same folder as the directory version
(`lionrapid-translation`), so WordPress treats the two as one plugin: updates from the directory reach a ZIP install
too, and your settings stay.

## Connect

1. Open **Settings → Lionrapid** and click **Connect to Lionrapid**.
2. Approve the code in your Lionrapid account. The button opens it; you can also type the code at the address shown.
3. Back on the settings page, click **Confirm**.

Instead of connecting, you can paste the site key (`pk_…`) from your Lionrapid project under **Settings → Lionrapid**
and click **Save key**. Languages, the language switcher and excluded paths are set in your Lionrapid project and sync
to the site by themselves.

## Moving from an older ZIP

ZIP files before 1.3.1 installed into `wp-content/plugins/lionrapid`, a folder the directory does not update. Install
Lionrapid Translation from the directory and activate it: if the old copy is still active, the new one deactivates it
and keeps your site key and settings. Then delete the old copy from **Plugins**; the Plugins screen and
**Settings → Lionrapid** point it out while it is still installed. Do this on 1.4.2 or newer: before 1.4.2, deleting
the old copy also deleted the settings.

## Source

Every release ZIP contains the plugin's PHP source and the TypeScript sources of its own scripts (`assets/src/`). The
bundled scripts in `assets/dist/js/vendor/` come from the open-source
[Lionrapid SDK](https://github.com/LionRapid/lionrapid-sdk). Development happens in a private repository; each
release is published here and to the WordPress plugin directory from the same commit.

Bug reports and questions: [issues](https://github.com/LionRapid/lionrapid-wordpress/issues).

## License

MIT. See [LICENSE](LICENSE).
