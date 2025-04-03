# Yealink DSSKeys Configurator

A web-based tool for managing DSS (Direct Station Selection) keys on Yealink phones with expansion modules.

![image](https://github.com/user-attachments/assets/7f36d465-adfe-4d96-a673-a6cc86203c8e)


## Features

- **Visual Configuration**: Intuitive interface for managing DSS keys
- **Multiple Module Support**: Configure keys for up to 4 expansion modules
- **Key Types**: Supports BLF (Busy Lamp Field) and Transfer key types
- **Drag-and-Drop**: Easily rearrange keys between positions
- **Sorting**: Alphabetical sorting of keys while preserving locked positions
- **Import/Export**: Work with Yealink's native configuration format
- **Responsive Design**: Works on desktop and mobile devices

## Usage

### Basic Operations

1. **Add Modules**: Click "Add Module" to create new expansion modules
2. **Configure Keys**:
   - Click "Add Key" to add new DSS keys
   - Set key properties (Label, Extension, Type)
   - Drag to rearrange keys
   - Lock important keys to preserve their positions
3. **Import/Export**:
   - Paste existing Yealink config to import
   - Export to get Yealink-compatible configuration text

### Key Properties

Each DSS key supports:
- **Label**: Display name (max 20 chars)
- **Extension**: Phone extension number
- **Type**: 
  - BLF (Busy Lamp Field) - shows status and allows one-touch calling
  - Transfer - initiates call transfer
- **Lock**: Prevent key from being moved or sorted

## Installation

No installation required - runs directly in browser:

1. Download `index.html`
2. Open in any modern web browser
3. Start configuring!

For development:
```bash
python3 -m http.server 8000
```
Then open http://localhost:8000

## Configuration File Format

The tool works with Yealink's native format:
```
expansion_module.1.key.1.extension=1001
expansion_module.1.key.1.label=John Doe
expansion_module.1.key.1.line=1
expansion_module.1.key.1.type=16
expansion_module.1.key.1.value=1001
```

## Supported Devices

Tested with:
- Yealink T4x series (T41P, T42G, T46G, T48G)
- Yealink T5 series (T54W, T57W)
- Expansion modules (EXP20, EXP40, EXP50)

## License

MIT License

## Credits

Developed by [Jonathan Gauthier](mailto:Jonathan@paretobiz.com)  
© 2025 [Pareto Business Solutions](https://paretobiz.com)

[![Buy me a Coffee](https://github.com/user-attachments/assets/39b6b3e4-2a35-4e8a-9fb4-99da59ea615a)](https://buymeacoffee.com/jonathangauthier)
