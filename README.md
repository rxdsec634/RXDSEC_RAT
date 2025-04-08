# RXDSEC RAT: Advanced Android Remote Access Tool

![RXDSEC RAT Banner](static/img/rxdsec_banner.png)

**Created by [@rxdsec](https://t.me/rxdsec)**

## Overview

RXDSEC RAT is an advanced Android Remote Access Tool featuring cross-platform compatibility, powerful surveillance capabilities, and sophisticated anti-detection mechanisms. This tool provides a comprehensive command and control (C2) platform for managing Android devices remotely.

> **Educational Purpose Statement**: This tool is developed for educational and research purposes only. It demonstrates advanced techniques in cybersecurity, network communications, and Android system internals. Use of this software against systems without explicit permission is illegal.

## Core Features

### 🔒 Advanced Anti-Detection

- **Cross-Platform Compatibility**: Works on Android, Windows, Linux, and macOS
- **Emulator Detection**: Advanced checks to identify virtual environments
- **Anti-Debugging**: Multiple layers of protection against analysis
- **Process Hiding**: Conceals presence from task managers
- **String Encryption**: Prevents signature-based detection
- **Timing-Based Evasion**: Counters behavioral analysis
- **Sandbox Detection**: Identifies security research environments
- **Hardware Fingerprint Spoofing**: Masks device identity

### 📱 Comprehensive Surveillance

- **Screen Capture**: Real-time screen monitoring
- **Camera Access**: Front/rear camera image capture
- **Microphone Recording**: Audio surveillance capabilities
- **Location Tracking**: GPS/network-based positioning
- **SMS Interception**: View incoming/outgoing messages
- **Call Logging**: Monitor phone calls
- **Contacts Extraction**: Access contact information
- **Keylogging**: Record user input across applications

### 💻 Command & Control

- **Web-Based Interface**: Modern cyberpunk-themed dashboard
- **Multi-Device Management**: Control multiple targets
- **Real-Time Updates**: Live device status information
- **Command Queue**: Scheduled task execution
- **File Transfer**: Remote file management
- **Shell Access**: Execute commands remotely
- **Persistence**: Survive device reboots
- **Cross-Platform C2**: Single interface for all platforms

### 🛠️ APK Payload Generation

- **APK Binding**: Inject into legitimate applications
- **Customization**: Configurable payload options
- **Persistence Methods**: Multiple startup techniques
- **Android Compatibility**: Supports Android 5.0-15
- **Obfuscation**: Evades signature detection
- **Version-Specific Bypasses**: Counters security measures

## Technical Specifications

- **Server**: Python 3.11+, Flask, SQLAlchemy, PostgreSQL
- **Client**: Cross-platform Python implementation
- **Communication**: Encrypted WebSockets/HTTPS
- **Security**: End-to-end encryption, HMAC verification
- **Persistence**: Platform-specific persistence methods
- **UI**: Responsive web interface with cyberpunk theme
- **Compatibility**: Android 5.0-15 (API 21-35)

## Installation

For detailed installation instructions, see [docs/INSTALLATION.md](docs/INSTALLATION.md).

### Quick Start

1. Install dependencies:
   ```
   chmod +x install_dependencies.sh
   sudo ./install_dependencies.sh
   ```

2. Configure database:
   ```
   export DATABASE_URL="postgresql://username:password@localhost/rxdsec"
   ```

3. Start the server:
   ```
   python main.py
   ```

4. Access the control panel:
   ```
   http://localhost:5000
   ```

## Documentation

- [Installation Guide](docs/INSTALLATION.md)
- [Requirements](docs/REQUIREMENTS.md)
- [Usage Guide](docs/USAGE.md)
- [Architecture Overview](docs/ARCHITECTURE.md)
- [API Reference](docs/API_REFERENCE.md)
- [APK Payload Generation](docs/APK_PAYLOAD_GENERATION.md)
- [Security Considerations](docs/SECURITY.md)
- [Troubleshooting](docs/TROUBLESHOOTING.md)

## Cross-Platform Compatibility

RXDSEC RAT has been enhanced with cross-platform compatibility:

- **Android**: Full feature support (API 21-35)
- **Windows**: Surveillance and C2 capabilities
- **Linux**: Command execution and data exfiltration
- **macOS**: System monitoring and control

## Advanced Usage

For detailed usage instructions, see [docs/USAGE.md](docs/USAGE.md).

## Version-Specific Bypasses

RXDSEC RAT includes bypass techniques for security measures in Android 10-15:

- **Android 10 (API 29)**: Scoped storage, background location
- **Android 11-12 (API 30-31)**: Package visibility, storage access
- **Android 13 (API 33)**: Notification permissions, background sensors
- **Android 14-15 (API 34-35)**: Screen intents, background process

## Security Considerations

- All communications are encrypted (AES-256-GCM)
- Authentication uses HMAC and secure tokens
- Payload templates include security validation
- For more details, see [docs/SECURITY.md](docs/SECURITY.md)

## Disclaimer

This software is provided for educational and research purposes only. The developer assumes no liability and is not responsible for any misuse or damage caused by this program. Users are responsible for ensuring compliance with local laws and regulations.

## License

Copyright © 2023-2025 RXDSEC. All rights reserved.

This software is provided "as is," without warranty of any kind. The use of this software for attacking targets without prior mutual consent is illegal.