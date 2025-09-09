# Encrypted DNS Profile Generator for Apple Devices

A simple, client-side web application to generate encrypted DNS profiles (.mobileconfig) for iOS, iPadOS, and macOS. This tool helps you enhance your online privacy by encrypting your DNS queries, preventing third parties from snooping on the websites you visit.

**Live App:** [https://realgauravmehta.github.io/Encrypted-DNS/](https://realgauravmehta.github.io/Encrypted-DNS/)

-----

## Features

  * **Easy to Use:** A user-friendly interface to create custom DNS profiles in seconds.
  * **Supports DoH & DoT:** Choose between DNS-over-HTTPS (DoH) and DNS-over-TLS (DoT) protocols.
  * **Provider Presets:** Pre-configured settings for popular DNS providers like Cloudflare, Google, NextDNS, and more.
  * **Custom Configuration:** Flexibility to use any DNS provider by entering a custom DoH or DoT server URL.
  * **Advanced Options:** Specify server IP addresses for more complex configurations.
  * **Client-Side Generation:** All processing is done in your browser. No data is sent to any server, ensuring your privacy.
  * **Modern UI:** A clean and responsive design with a dark theme.

-----

## How to Use

1.  **Open the Generator:** Navigate to the [Encrypted DNS Profile Generator](https://realgauravmehta.github.io/Encrypted-DNS/).
2.  **Profile Name:** Give your DNS profile a descriptive name (e.g., "My Secure DNS").
3.  **Provider Preset:**
      * Select a provider from the dropdown list (e.g., Cloudflare, Google).
      * If your provider requires a Resolver ID (like NextDNS or Control D), the Resolver ID field will appear. Paste your unique ID into this field.
      * For a custom provider, select "Custom" and manually enter the DoH or DoT server details.
4.  **DNS Protocol:** Choose between DNS-over-HTTPS (DoH) or DNS-over-TLS (DoT). The form will update to show the relevant input field.
5.  **(Optional) Advanced Settings:** If needed, you can add specific server IP addresses in the "Advanced Settings" section.
6.  **Generate & Download:** Click the "Generate & Download Profile" button. A `.mobileconfig` file will be downloaded to your device.
7.  **Install the Profile:**
      * **iOS/iPadOS:** Open the downloaded file. Go to **Settings \> General \> VPN & Device Management** and tap on the downloaded profile to install it.
      * **macOS:** Open the downloaded file. Go to **System Settings \> Privacy & Security \> Profiles** and double-click the profile to install it.

-----

## Supported DNS Providers

The generator includes presets for the following trusted DNS providers:

| Provider | DoH URL | DoT Hostname |
| :--- | :--- | :--- |
| Cloudflare | `https://cloudflare-dns.com/dns-query` | `1dot1dot1dot1.cloudflare-dns.com` |
| Google | `https://dns.google/dns-query` | `dns.google` |
| Quad9 | `https://dns.quad9.net/dns-query` | `dns.quad9.net` |
| NextDNS | `https://dns.nextdns.io/YOUR-ID` | `YOUR-ID.dns.nextdns.io` |
| Control D | `https://dns.controld.com/YOUR-ID` | `YOUR-ID.dns.controld.com` |
| Mullvad DNS | `https://dns.mullvad.net/dns-query` | `dns.mullvad.net` |
| OpenDNS | `https://doh.opendns.com/dns-query` | `dns.opendns.com` |

-----

## What is Encrypted DNS?

Normally, when you visit a website, your device sends a DNS query in plain text. This means your Internet Service Provider (ISP) and anyone else on the network can see which websites you are trying to access.

**Encrypted DNS** (using protocols like DoH and DoT) wraps your DNS queries in a layer of encryption. This makes it much more difficult for third parties to monitor your internet activity, significantly improving your privacy and security online.

-----

## License

This project is licensed under the MIT License. See the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.
