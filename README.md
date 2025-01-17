# hass-fontawesome

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

Use free icons from the [fontawesome](https://fontawesome.com) set in Home-assistant.

# Installation instructions

- Install using [HACS](https://hacs.xyz) (Or copy the contents of `custom_components/fontawesome/` to `<your config dir>/custom_components/fontawesome/`.)

- Restart Home Assistant

- Go to your integrations configuration and add FontAwesome
![Install](https://user-images.githubusercontent.com/1299821/68902965-f731fc80-0739-11ea-8712-9329243ca8f6.png)

- Open the settings for the new FontAwesome integration

- Click the Options gear (red arrow below) and select which icon sets to load
![Options](https://user-images.githubusercontent.com/1299821/68903005-1466cb00-073a-11ea-9d6d-57bc5528ef88.png)


# Icon sets

The icons are divided into three sets.

- Solid
- Regular
- Brands

Each set will add a few hundred kilobytes to the ammount of data that's downloaded to your browser every time you open up your Home Assistant interface, so to save on your data plan, make sure to only select the ones you actually need.

# Usage

Find the icon you want in the [gallery](https://fontawesome.com/icons?d=gallery&m=free).

The three icon sets have different prefixes: `fas:`, `far:` and `fab:` respectively.

So,

- to get a solid heart, use `fas:heart`
- to get a heart outline, use `far:heart`
- to get the twitter symbol, use `fab:twitter`

The icons are useable anywhere in Home Assistant - not only in lovelace.

# FAQ

### Can I use this with my Pro icon set?

You probably can, but you'll need to recompile things yourself.

I do not own the Pro Icon set, so I don't even know what structure it has.

You may be able to find some helpful information [here](https://fontawesome.com/how-to-use/on-the-web/setup/using-package-managers).

I also know that people have had success with Pro Icons and the [previous version of this integration](https://github.com/thomasloven/hass-fontawesome/tree/4ed9d97bbb1621d4ff68a0053add29294529f5b0).

PRs with the process are very welcome.

### Can I set this up in configure.yaml instead?

Yes.

```
fontawesome:
  regular:
  solid:
  brands:
```

Just remove the lines for the icon sets you don't want.

---
<a href="https://www.buymeacoffee.com/uqD6KHCdJ" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/white_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
