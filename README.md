# FireBot ID/KEY Writer

Phone-side web page for writing device ID and KEY to FireBot products via ESP32 OTW tool.

## Usage

1. ESP32 OTW tool detects blank ID/KEY on target device
2. Open this page on your phone
3. Scan device QR code to get the ubilinkId
4. Page fetches the matching key from the API
5. Page sends ID+KEY to ESP32 via local network
6. Press START on ESP32 to write

## Live URL

After deploying to GitHub Pages, visit:
`https://<username>.github.io/firebot-id-key-writer/`

## Notes

- Camera permission requires HTTPS (provided by GitHub Pages).
- The KEY API and ESP32 use HTTP. To allow the page to call them from HTTPS,
  enable Chrome flag `chrome://flags/#unsafely-treat-insecure-origin-as-secure`
  and add the API origin + ESP32 IP origin to the allowlist.
