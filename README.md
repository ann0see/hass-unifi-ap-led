# UniFi AP LED Control for Home Assistant

![GitHub Release](https://img.shields.io/github/v/release/omgitslurch/hass-unifi-ap-led) ![GitHub top language](https://img.shields.io/github/languages/top/omgitslurch/hass-unifi-ap-led) [![CodeFactor](https://www.codefactor.io/repository/github/omgitslurch/hass-unifi-ap-led/badge)](https://www.codefactor.io/repository/github/omgitslurch/hass-unifi-ap-led)
 ![GitHub Repo stars](https://img.shields.io/github/stars/omgitslurch/hass-unifi-ap-led) [!["Buy the author A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/omgitslurch)

This integration allows Home Assistant to control the **status LEDs** on UniFi Access Points (APs), including:

- 🔄 Turning the LED on/off via a `switch`
- ✴️ Flashing the LED for 2 minutes via a `button` 
- ⚙️ Fully configurable via the Home Assistant UI

> **Note** ⚠️ This is an early **Beta** release. In theory, it supports both UDMs and self-hosted controllers. However, I only have a self-hosted controller available for testing, so UDM support is unconfirmed.

---

## Installation

- Add the repository to HACS  
<a href="https://my.home-assistant.io/redirect/hacs_repository/?category=integration&amp;repository=hass-unifi-ap-led&amp;owner=omgitslurch" rel="nofollow"><img src="https://my.home-assistant.io/badges/hacs_repository.svg" alt="Open your Home Assistant instance and open a repository inside the Home Assistant Community Store."></a>
- Install **UniFi AP LED Control**
- Restart Home Assistant

---

## Configuration

You will need:
- UniFi Controller IP/hostname
- Username and password (use a local account with limited permissions)
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

⚠️ This integration allows you to disable SSL verification when connecting to the UniFi controller. If you do so, ensure your network is secure and that credentials are protected.

---

## Disclaimer

This integration is provided "as is" and without any warranty. Use it at your own risk. The authors are not responsible for any damage, data loss, or issues that may arise from its use.

---

## License

MIT License
