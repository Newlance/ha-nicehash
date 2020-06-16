# NiceHash Home Assistant Integration

[![GitHub Release][releases-shield]][releases]
[![License][license-shield]](LICENSE)

[![hacs][hacsbadge]][hacs]
![Project Maintenance][maintenance-shield]
[![BuyMeCoffee][buymecoffeebadge]][buymecoffee]

[![Discord][discord-shield]][discord]
[![Community Forum][forum-shield]][forum]

_Component to integrate with [NiceHash][nicehash]_

**This component will set up the following platforms.**

Platform | Description
-- | --
`sensor` | Show info from NiceHash API

## Installation

1. Using the tool of choice open the directory (folder) for your HA configuration (where you find `configuration.yaml`).
1. If you do not have a `custom_components` directory (folder) there, you need to create it.
1. In the `custom_components` directory (folder) create a new folder called `nicehash`.
1. Download _all_ the files from the `custom_components/nicehash/` directory (folder) in this repository.
1. Place the files you downloaded in the new directory (folder) you created.
1. Generate [NiceHash][nicehash] API key
    - Supported API Permissions
      - Wallet Permissions > View balances...
      - Mining Permissions > View mining data...
    - See this [repository](https://github.com/nicehash/rest-clients-demo) for assistance
1. Add `nicehash` to `configuration.yaml`
    ```
    nicehash:
      organization_id: <org_id>
      api_key: <api_key_code>
      api_secret: <api_secret_key_code>
    ```
1. Restart Home Assistant

Using your HA configuration directory (folder) as a starting point you should now also have this:

```text
custom_components/nicehash/translations/en.json
custom_components/nicehash/__init__.py
custom_components/nicehash/const.py
custom_components/nicehash/manifest.json
custom_components/nicehash/sensor.py
```

<!---->

## Contributions are welcome!

If you want to contribute to this please read the [Contribution guidelines](CONTRIBUTING.md)


[nicehash]: https://nicehash.com
[buymecoffee]: https://www.buymeacoffee.com/brianberg
[buymecoffeebadge]: https://img.shields.io/badge/buy%20me%20a%20coffee-donate-yellow.svg?style=for-the-badge
[commits-shield]: https://img.shields.io/github/commit-activity/y/brianberg/ha-nicehash.svg?style=for-the-badge
[commits]: https://github.com/brianberg/ha-nicehash/commits/master
[hacs]: https://github.com/custom-components/hacs
[hacsbadge]: https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge
[discord]: https://discord.gg/Qa5fW2R
[discord-shield]: https://img.shields.io/discord/330944238910963714.svg?style=for-the-badge
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg?style=for-the-badge
[forum]: https://community.home-assistant.io/
[license-shield]: https://img.shields.io/github/license/brianberg/ha-nicehash?style=for-the-badge
[maintenance-shield]: https://img.shields.io/badge/maintainer-Brian%20Berg%20%40brianberg-blue.svg?style=for-the-badge
[releases-shield]: https://img.shields.io/github/v/release/brianberg/ha-nicehash?style=for-the-badge
[releases]: https://github.com/brianberg/ha-nicehash/releases
