# Humly Device API Test

A simple web page for testing Humly Room Display device API endpoints in URL signage mode.

## Usage

1. Open the test page in a browser on the device or access it via the URL signage feature
2. The API endpoint defaults to `http://127.0.0.1:3000` (device localhost)
3. Use the controls to test various device functions

## Available Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/serial` | GET | Read device serial numbers |
| `/api/reboot` | POST | Reboot the device |
| `/api/backlight` | POST | Set screen brightness (0-255) |
| `/api/leds` | GET | Read current LED colors |
| `/api/leds` | POST | Set LED colors (halo/logo/all) |
| `/api/settings` | GET | Read device settings |
| `/api/settings` | PATCH | Update device settings |
| `/api/rfid` | GET | Scan RFID/NFC tag |
| `/api/rfid` | POST | Scan with callback URL |
| `/api/firmware` | GET | Check firmware version |
| `/api/logs` | GET | Retrieve device logs |

## Security Note

The device API only accepts connections from localhost (`127.0.0.1`, `::1`). This test page must be loaded on the device itself to work.

## GitHub Pages

This page can be hosted on GitHub Pages and loaded as a URL signage source on Humly devices.
