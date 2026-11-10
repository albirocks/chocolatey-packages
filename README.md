# chocolatey-packages

Source code of the Chocolatey community packages maintained by **[Tabularasa](https://community.chocolatey.org/profiles/Tabularasa)**.

| Package | Description | Chocolatey |
|---|---|---|
| [lenovo-commercial-vantage](lenovo-commercial-vantage) | Lenovo Commercial Vantage – BIOS, firmware and driver updates for ThinkPad, ThinkCentre, ThinkStation and ThinkBook. Successor of Lenovo System Update (EOL March 2027). | [community.chocolatey.org](https://community.chocolatey.org/packages/lenovo-commercial-vantage) |

## How these packages work

- Installers are **downloaded from the vendor's official servers** at install time and verified with a **SHA256 checksum**.
- No vendor binaries are stored in this repository or in the packages.
- Every package has an `update-package.ps1` that takes the new vendor download link, calculates the checksum, sets the version and builds the `.nupkg`.

## Quick start

```powershell
choco install lenovo-commercial-vantage -y                      # full Commercial Vantage
choco install lenovo-commercial-vantage -y --params "'/Lite'"   # System Update function only
```

## Issues

Problems with a package (not with the software itself)? Please open an [issue](../../issues) or leave a comment on the package page on community.chocolatey.org.

## Disclaimer

These packages are not affiliated with or endorsed by the software vendors. All trademarks belong to their respective owners. By installing a package you accept the vendor's license terms.
