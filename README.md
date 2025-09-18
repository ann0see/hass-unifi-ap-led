# UniFi AP LED Control for Home Assistant

![GitHub Release](https://img.shields.io/github/v/release/omgitslurch/hass-unifi-ap-led) ![GitHub top language](https://img.shields.io/github/languages/top/omgitslurch/hass-unifi-ap-led) [![CodeFactor](https://www.codefactor.io/repository/github/omgitslurch/hass-unifi-ap-led/badge)](https://www.codefactor.io/repository/github/omgitslurch/hass-unifi-ap-led)
 ![GitHub Repo stars](https://img.shields.io/github/stars/omgitslurch/hass-unifi-ap-led) [!["Buy the author A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/omgitslurch)

This integration allows Home Assistant to control the **status LEDs** on UniFi Access Points (APs), including:

- 🔄 Turning the LED on/off via a `light entity`
- ✴️ Flashing the LED for 2 minutes via a `button entity` 
- ⚙️ Fully configurable via the Home Assistant UI

---

## Requirements
- Home Assistant 2023.1.0 or later (recommended)
- HACS (Home Assistant Community Store)
- A UniFi controller (self-hosted, UDM or Cloud Gateway, though UDM and Cloud Gateway support is untested)

---

## Installation

- Search for "UniFi AP LED Control" in HACS
- Install **UniFi AP LED Control**
- Restart Home Assistant

---

## Configuration

You will need:
- UniFi Controller IP/hostname
- Username and password (use a local account with no MFA for least risk). If an account has MFA enabled, it will fail.
- Site ID (usually `default`)

---

## Flash Button

Triggers the `locate` command to blink the AP LED for 2 minutes — useful for physically identifying devices.

---

## Switch

Turns the AP's LED on or off.  
Note: This does **not** disable the actual Wi-Fi functionality.

---

## Security

- ⚠️ This integration allows you to disable SSL verification when connecting to the UniFi controller. If you do so, ensure your network is secure and that credentials are protected.
- You should not use your main ui.com account. Create a local account on your Controller for the Integration to use with no MFA enabled.

---

## Troubleshooting

- **Connection errors**: Ensure the controller IP/hostname is correct and reachable.
- **Authentication errors**: Verify the username/password and ensure the account has sufficient permissions, and does **NOT** have MFA enabled.
  
---

## Disclaimer

This integration is provided "as is" and without any warranty. Use it at your own risk. The authors are not responsible for any damage, data loss, or issues that may arise from its use.

---

## License

MIT License
