# Data and compatibility

[Overview](../../README.md) · [User guide](user-guide.md) · [한국어](../ko/technical-reference.md)

This public reference describes Butim **v1.9.2** installation requirements and user-visible data behavior. Butim's source code and internal implementation are not provided in this repository.

## Installation requirements

Butim supports Windows 10/11 x64 and requires .NET 10.0 Desktop Runtime (x64). `Butim_Setup.exe` includes the runtime installer and installs it if needed. Butim installs for the current user; runtime installation may require administrator approval.

Download the installer from [GitHub Releases](https://github.com/funk80/Butim/releases/latest). GitHub's automatically generated source archives are snapshots of this documentation repository, not the Windows installer or the application source.

## Note files and storage

Notes and settings are stored locally under `%APPDATA%\Butim\`. The [user guide](user-guide.md#data-and-installation) lists the storage locations and uninstall behavior. Local storage alone is not a claim of encryption, password protection, or a backup service.

Export creates a `.butim` file on the desktop. Importing it successfully returns the note to the app and deletes the imported file. Keep a separate copy when you need to retain an exported archive. A note's editing lock prevents text changes; it does not restrict moving, deleting, or access to its files.

Use the app's export and import controls to transfer individual notes. This repository does not publish an editable file schema or promise compatibility with other apps' note formats.

## Settings after an update

Older settings may not contain options added in later versions. In the documented v1.9.2 behavior:

- An unspecified peel-off action defaults to Export to desktop.
- If no title-bar icon preferences are saved, all icons are shown.
- If no language preference is saved, Korean Windows selects Korean; other display languages select English.

Review General settings after an update if the language, title bar, or peel-off behavior differs from what you expect. See [Settings](user-guide.md#settings) for the controls. This is not a guarantee that every future version will preserve all data or settings formats.

## Help and reporting

Use [Bug Report or Feature Request](https://github.com/funk80/Butim/issues/new/choose) for ordinary problems and suggestions, with sample data only. For security concerns, follow [SECURITY.md](../../SECURITY.md). Usage rights are defined in [LICENSE.txt](../../LICENSE.txt).
