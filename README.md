# Windows Wi-Fi Key Thief
This Windows batch script is designed to extract and save access keys for Wi-Fi networks saved on your system. It scans and records data related to wireless network access in a file named `wifi_keys.txt`. Please note that using this script may require permissions and compliance with data protection and privacy laws.

**Author:** [d1yorhay](https://github.com/d1yorhay)

## Prerequisites
Before using this script, ensure you have the following:

- Windows operating system
- Administrator or elevated privileges

## Usage

1. Download the script to your computer.
```batch
git clone https://github.com/d1yorhay/windows-wifi-key-thief
```
2. Open the script folder.
```batch
cd windows-wifi-key-thief
```
3. Run the script.
```batch
script.bat
```

> You can also run the script from Explorer
## How It Works

The script performs the following steps:

1. It sets the local environment variable to enable delayed expansion and changes the code page to 65001 to support UTF-8 characters.
2. It uses the `netsh wlan show profiles` command to list the Wi-Fi network profiles and saves the output to a temporary file named `temp`.
3. It processes the `temp` file, extracting Wi-Fi network names and obtaining their access keys.
4. The extracted data is appended to the `wifi_keys.txt` file, and a signature is added to indicate the script's authorship.

> Please exercise caution and ensure you have the necessary permissions to run this script, as it may involve accessing sensitive information.

## Disclaimer

This script is provided for educational and informational purposes only. Any use of this script to access Wi-Fi networks without authorization may be illegal and unethical. Always respect privacy and adhere to the laws and regulations in your jurisdiction.

**Use this script responsibly and only on networks for which you have explicit permission to access. The author and contributors are not responsible for any misuse or illegal activities involving this script.**

## License

This script is distributed under the [MIT License](LICENSE).

For questions, suggestions, or issues, please [open an issue](https://github.com/d1yorhay/windows-wifi-key-thief/issues) on the GitHub repository.

Enjoy responsibly!
