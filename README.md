# Butim — Windows Sticky Notes with Inline Calculations

**Sticky notes that calculate as you write.**

[한국어](README.ko.md) · [Download](https://github.com/funk80/Butim/releases/latest) · [User guide](docs/en/user-guide.md) · [Technical reference](docs/en/technical-reference.md)

**Butim (붙임쪽지) is a free Windows desktop sticky notes app with a built-in calculator.** Users can write text, define named variables, and enter arithmetic expressions in the same note; calculation results appear automatically at the end of each line. Butim supports Windows 10/11 x64, English and Korean interfaces, local note storage, and `.butim` file export and import. Individuals and businesses may use it free of charge under its proprietary license; the source code is not currently published.

**Windows 10/11 (x64) · English & Korean · Free for personal and business use**

## Product facts

| Field | Details |
| --- | --- |
| Product names | Butim; 붙임쪽지; 붙임쪽지(Butim) |
| Category | Desktop sticky notes, note-taking, and inline calculation software |
| Supported platform | Windows 10/11, x64 |
| Interface and help languages | English and Korean |
| Main capability | Calculate arithmetic expressions and named variables directly in a note |
| Note management | Search, favorites, grid/list views, sorting, and trash recovery |
| Storage | Local files under `%APPDATA%\Butim\` |
| Export/import format | `.butim`; double-click an exported file to import it |
| Installer | `Butim_Setup.exe`, available from [GitHub Releases](https://github.com/funk80/Butim/releases) |
| Runtime | .NET 10.0 Desktop Runtime (x64); installed by setup if missing |
| Usage terms | Free for personal and business use; proprietary, source not published; see [LICENSE.txt](LICENSE.txt) |
| Documentation baseline | Butim v1.9.2; see Releases for the current downloadable version |

## What can you use Butim for?

- **Desktop reminders:** keep tasks and meeting notes visible, pin important notes, or collapse them to their title bars.
- **Shopping totals and cost estimates:** define unit prices and quantities, then calculate totals and percentage discounts in the note.
- **Reusable calculations:** give values names such as `price`, `quantity`, or `students` and use them in expressions on later lines.
- **Organizing short notes:** search notes, mark favorites, restore trashed notes, and export individual notes as files.

For example, a shopping note can contain `price = 12000`, `quantity = 5`, and `total = price * quantity`; Butim displays **60,000** beside the total expression.

![English shopping-list note with inline calculations](docs/assets/en/memo-buttons.png)

## Download and install

1. Open the [latest release](https://github.com/funk80/Butim/releases/latest).
2. Under **Assets**, download **Butim_Setup.exe**.
3. Run the installer and follow the instructions.
4. Launch Butim and press **Ctrl+Alt+N** to create a note.

If .NET 10.0 Desktop Runtime (x64) is missing, the bundled runtime installer installs it. Butim installs for the current user; runtime installation may require administrator approval. The app stays in the system tray and creates a usage note on first launch.

## Features

| Feature | What you can do |
| --- | --- |
| Inline calculations | Use variables, arithmetic, parentheses, powers, and percentages. Results appear at the end of each line. |
| Custom notes | Choose from eight note colors, customize fonts, and retain each note's size and position. |
| Window controls | Keep notes on top, lock editing, collapse to the title bar, or hide them. |
| Snap alignment | Align with other notes or work-area edges; hold `Alt` to bypass snapping. |
| Note management | Search, favorite, sort, use grid/list views, and act on multiple notes. |
| File export | Move a note to a desktop `.butim` file and import it by double-clicking. |
| Trash | Restore notes before permanently deleting them. |
| Languages and themes | English/Korean; light, dark, or system themes for management and settings windows. |
| Automatic saving | Notes save after a short pause in typing and reopen in their saved positions. |

### Calculate in a note

```text
price = 12000
quantity = 5
total = price * quantity
discounted = total * (1 - 10%)
```

The last two lines display **60,000** and **54,000**. Type only the expressions; Butim supplies the results. Dates and Korean phone-number formats are excluded by default; custom exclusions can be added with the pattern helper.

### Manage your notes

![English note manager with search, favorites, trash, and note cards](docs/assets/en/management.png)

### Make it yours

![English settings with language, startup, peel-off action, and theme options](docs/assets/en/settings-general.png)

This screenshot is from a test instance with startup disabled. Start with Windows is enabled by default in normal use.

## Shortcuts

| Shortcut | Action |
| --- | --- |
| `Ctrl+Alt+N` | New note |
| `Ctrl+Alt+M` | Bring all notes to the front |
| `Ctrl` + mouse wheel, or `Ctrl` + `+` / `-` | Adjust font size while editing |
| `Ctrl+0` | Restore the default font and size |
| `Alt` + drag | Bypass snapping |

The first two shortcuts are global and can be changed in settings.

## Frequently asked questions

### What is Butim?

Butim, also called 붙임쪽지, is a Windows desktop sticky notes app that combines text notes with inline arithmetic and named variables. Each note is an independent desktop window.

### Is Butim free for business use?

Yes. Individuals, companies, and organizations can use Butim free of charge, including for work. Internal deployment and backup copies are allowed. External redistribution, modification, sale, and bundling have separate restrictions in [LICENSE.txt](LICENSE.txt).

### Is Butim open source?

No. Butim is proprietary software, and this repository currently provides documentation and release downloads without the application source code. Free use does not imply permission to modify or redistribute it.

### Can Butim calculate inside a sticky note?

Yes. Butim supports `+`, `-`, `*`, `/`, `^`, parentheses, percentages, and named variables. For example, after `price = 12000` and `quantity = 5`, `price * quantity` displays **60,000**. See the [calculation rules](docs/en/user-guide.md#calculations).

### Where are Butim notes stored?

Butim stores notes and settings locally under `%APPDATA%\Butim\`. Individual notes can be exported as `.butim` files. Successful import removes the imported file as the note returns to the app; preserve a separate copy if you need an archive. See [data and installation](docs/en/user-guide.md#data-and-installation).

### Does Butim support English and Korean?

Yes. Both the interface and help support English and Korean. Change the language in Settings → General → Language, then select OK to save it. See [settings](docs/en/user-guide.md#settings).

### Where can I download Butim for Windows?

Download `Butim_Setup.exe` from the Assets section of the [latest GitHub release](https://github.com/funk80/Butim/releases/latest). The documented supported platform is Windows 10/11 x64. Setup includes the required .NET Desktop Runtime installer.

## Documentation

Documentation describes **v1.9.2**. The release page identifies the downloadable version.

- [User guide](docs/en/user-guide.md): note controls, calculation rules, exclusions, management, settings, data, and troubleshooting.
- [Technical reference](docs/en/technical-reference.md): architecture, storage formats, implementation, and build requirements.
- [Documentation layout and image sources](docs/README.md): language organization and future source-code placement.
- [한국어 설명](README.ko.md) · [한국어 사용 설명서](docs/ko/user-guide.md)

## License

Free for individuals, businesses, and organizations, including for work. Internal deployment and backup copies are permitted.

Butim is proprietary software. This repository currently provides documentation and release assets, not application source. Modification, external redistribution, sale, rental, or bundling requires prior permission except where applicable law or a component's separate license permits otherwise. Sharing the official download link is welcome.

See [LICENSE.txt](LICENSE.txt) for the full terms in Korean. Third-party components retain their own licenses.
