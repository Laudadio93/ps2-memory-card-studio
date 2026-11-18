# PS2 Memory Card Studio

Create PS2 virtual memory cards from multiple save files on Windows.

## Download

Download the **Windows ZIP** from [Releases](../../releases/latest), extract it, and run `PS2 Memory Card Studio.exe`. Python is not required for the bundled executable. The release also includes a source archive.

## Features

- Import PSU, MAX, CBS, SPS, XPS, and PS2 PSV saves.
- Combine multiple saves on one card.
- Choose ECC or non-ECC and 8, 16, 32, or 64 MiB.
- Blank card templates are bundled. Choose the output folder in the app.
- The app processes saves locally and backs up an existing output before replacement.

ECC images use `.PS2`; non-ECC images use `.VMC`. For Apollo Save Tool, copy the finished card to `/PS2/VMC/` on the USB drive. Compatibility depends on the target setup and saves.

The app checks the selected capacity and reports saves it could not read or duplicate save folders. Read the included guide for setup and troubleshooting.

## Credits

The PS2 filesystem and save-format engine is adapted from [PS2 Memory Card Manager](https://github.com/lawlmoeaung/ps2-memory-card-manager), including original work by Ross Ridge. Its upstream notices and Unlicense text are included in the downloads.
