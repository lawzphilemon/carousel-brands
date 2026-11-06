# carousel-brands

Brand profiles for the [carousel-plugin](https://github.com/lawzphilemon/carousel-plugin): one folder per brand under `brands/<slug>/` with `brand.json`, fonts, and logos.

Currently included:

| Brand | Folder |
|---|---|
| Truemission | `brands/truemission/` |

## Use

Clone this repo into the folder the carousel plugin treats as its workspace, so that `brands/` sits next to `carousel-output/`:

```bash
git clone https://github.com/lawzphilemon/carousel-brands.git carousel
cd carousel
# brands/truemission/brand.json is now where the plugin looks for it
```

## Before you use it

- `tracking.sheet_id` in `brand.json` is a placeholder (`REPLACE_WITH_YOUR_SHEET_ID`). Put your own Google Sheet ID there, or remove the `tracking` block if you do not log carousels to a sheet.
- Never commit `carousel-output/` here. It holds generated posts and is kept out of this repo on purpose.
- The brand rules in `brand.json` (voice, hard rules, call to action) belong to one brand. Change them before using the profile for anything else.

## Licenses

- `brands/*/fonts/OpenSans-Variable.ttf`: Open Sans, SIL Open Font License 1.1 (see `brands/*/fonts/OFL.txt`).
- Logos and brand rules: all rights reserved by the brand owner. They are published for testing the plugin and are not licensed for reuse.
