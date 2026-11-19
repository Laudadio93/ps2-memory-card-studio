# PS1 & PS2 Memory Card Studio

Create PlayStation and PlayStation 2 virtual memory cards from your saves in one standalone Windows application. Choose the PS1 or PS2 tab, add saves, review the card format, and choose where to save the result.

**[Download the Windows ZIP](https://github.com/Laudadio93/ps2-memory-card-studio/releases/latest)**, extract it, and open **PS1 and PS2 Memory Card Studio.exe**. The executable includes its runtime and blank card templates. Users do not need Python or a separate memory-card utility.

## What's new

- **PS1 Memory Card Studio** now sits alongside the existing PS2 editor in the same application.
- Create a blank PS1 card, import multiple MCS saves, or bring saves across from standard raw 128 KiB PS1 memory-card images.
- Export a raw PS1 card as MCR, MCD, VM1, or VMC and see the available 15 save blocks.
- Switch between dedicated PS1 and PS2 views with system-specific card previews, controls, output names, and Apollo guidance.
- The Windows application uses the custom PlayStation memory-card icon and includes both sets of blank templates.

## PS2 cards

- Combine saves from PSU, MAX, CBS, SPS, XPS, and PS2 PSV files. Add files in multiple selections.
- Choose **8, 16, 32, or 64 MiB**, and select ECC or non-ECC. The selected capacity appears on the card preview.
- Export ECC cards as **.ps2** and non-ECC cards as **.vmc**.
- Check the selected capacity before creation. The app reports unreadable saves and duplicate save directories.
- Card output is staged to avoid replacing the destination with a partial card when space runs out.

For Apollo Save Tool, place a PS2 image in **/PS2/VMC/** on the USB drive.

## PS1 cards

- Create a blank card or combine **MCS** saves and saves from standard raw **128 KiB** cards.
- Export a raw card as **.mcr**, **.mcd**, **.vm1**, or **.vmc**.
- Review imported saves and the **15 usable 8 KiB blocks**. The app checks directory frames, checksums, file lengths, and block chains.
- Duplicate names, malformed saves, overlapping chains, and saves exceeding available blocks are reported.

For Apollo Save Tool, place a PS1 image in **/PS1/VMC/** on the USB drive. PS1 PSV and headered formats such as VMP are outside the PS1 importer.

## Using the app

1. Extract the Windows ZIP and open **PS1 and PS2 Memory Card Studio.exe**.
2. Select **PS1 Memory Card Studio** or **PS2 Memory Card Studio**.
3. Add your saves. In the PS2 view, choose ECC and capacity. In the PS1 view, choose a raw card extension.
4. Choose the output folder and filename, then create the card.
5. Copy the result to your target device. The output folder choice is remembered. An existing output is backed up before replacement.

Saves and card creation are processed on your PC. A successful import checks the card structure and source data. Gameplay and compatibility depend on the console, software, and individual save.

## Credits

- **Ross Ridge** wrote the original PS2 filesystem and save-format code. **lawlmoeaung and the PS2 Memory Card Manager contributors** maintain the adaptation used by this app. The upstream notice and Unlicense are included with the Windows ZIP. [PS2 Memory Card Manager](https://github.com/lawlmoeaung/ps2-memory-card-manager)
- **Martin Korth and PSX-SPX contributors** document the PS1 memory-card directory and block layout. [PSX-SPX](https://psx-spx.consoledev.net/)
- **bucanero and the Apollo Save Tool contributors** maintain the target save manager. [Apollo Save Tool for PS3](https://github.com/bucanero/apollo-ps3)
- **Microsoft and the .NET and WPF contributors**, the **Python Software Foundation**, **Tcl/Tk**, **Tom Schimansky and CustomTkinter contributors**, **darkdetect contributors**, and **PyInstaller contributors** provide the desktop and memory-editor runtimes. [WPF](https://github.com/dotnet/wpf) · [Python](https://www.python.org/) · [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) · [PyInstaller](https://pyinstaller.org/)
- **Laudadio93** maintains this application. PlayStation systems and marks belong to Sony Interactive Entertainment and their respective owners.

The original PS2-only release remains available in the release history.
