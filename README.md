# Tapr: Gesture-Driven Trackpad Control System

**Tapr** is an innovative open-source system for detecting and interpreting precise gestures using touch-sensing trackpads, translating them into configurable device control commands. Originally developed as a passion project to explore gesture recognition and hardware integration.

## What is Tapr?

Tapr bridges the gap between intuitive human interaction and device control by leveraging the capacitive sensors already present in modern trackpads. Instead of traditional button presses, app interactions, and keyboard commands, Tapr enables users to control devices through natural hand gestures—swipes, taps, and multi-finger interactions.

### Core Concept
The system is built on a layered architecture:
- **Gesture Detection**: Low-level trackpad event processing and gesture state management
- **Gesture Processing**: Real-time gesture recognition and classification
- **Device Control**: REST API integration for controlling smart devices (Govee API supported)

## Repositories

| Repository | Purpose | Status |
|---|---|---|
| **[Tapr-Trackpad](https://github.com/ZCW-Tapr/Tapr-Trackpad)** | Core gesture detection engine; reads raw trackpad events and processes them into actionable gestures | Python, Active |
| **[Tapr-Backend-Controller](https://github.com/ZCW-Tapr/Tapr-Backend-Controller)** | Backend service for device control; translates gestures into API commands for smart devices | Java/Spring Boot, Active |

## Getting Started

### Prerequisites
- Python 3.8+ (for trackpad module)
- Java 17+ (for backend controller)
- Linux system with trackpad support
- Smart devices compatible with control APIs (e.g., Govee Wi-Fi devices)

### Quick Setup
1. Clone both repositories:
   ```bash
   git clone https://github.com/ZCW-Tapr/Tapr-Trackpad.git
   git clone https://github.com/ZCW-Tapr/Tapr-Backend-Controller.git
   ```
2. See individual repository READMEs for installation and configuration

## Architecture Overview

```
Trackpad Events
    ↓
[Tapr-Trackpad] - Gesture Detection & State Management
    ↓
Gesture Data (HTTP/WebSocket)
    ↓
[Tapr-Backend-Controller] - Device Command Translation
    ↓
Smart Device APIs (Govee, etc.)
    ↓
Device Actions
```

## Key Features

✓ Real-time multi-touch gesture recognition  
✓ Configurable gesture mappings  
✓ REST API integration with smart device ecosystems  
✓ Minimal latency event processing  
✓ Extensible architecture for new device types  

## License & Commercial Terms

**Tapr is licensed under Commons Clause + MIT License**

### Free Use (Non-Commercial)
✅ Personal projects  
✅ Educational use (students, universities)  
✅ Non-profit organizations  
✅ Open-source community projects (non-revenue)  

### Commercial Use Requires Licensing
❌ Companies using Tapr in products/services  
❌ Commercial SaaS/consulting built on Tapr  
❌ Selling software/hardware incorporating Tapr  
❌ Enterprise deployments for profit  
→ **Must obtain a commercial license** from the Tapr organization:
Please reach out to Gabriel Cruz (Creator of Tapr) -> gabecruzpro@gmail.com

### Why This License?

Tapr represents original research and innovation in gesture-driven device control. We want to:
1. Keep it free for learners and hobbyists
2. Ensure companies pay for commercial use
3. Protect our intellectual property from being privatized
4. Fund ongoing development and support

---

## Getting a Commercial License

If you're interested in using Tapr commercially, contact us at:

**Email**: gabecruzpro@gmail.com 
**GitHub Issues**: [Tapr Organization](https://github.com/ZCW-Tapr)

Commercial licenses include:
- Legal right to use Tapr in your product/service
- Priority technical support
- Custom modifications and integrations
- Flexible per-deployment or per-seat pricing

---

## Full License Text

See [LICENSE](./LICENSE) in this repository for complete terms including:
- Detailed Commons Clause language
- MIT License full text
- Attribution requirements
- Disclaimer of warranties
- Commercial licensing contact information

## Contributing

We welcome contributions! Please:
1. Fork the relevant repository
2. Create a feature branch
3. Submit a pull request with clear documentation of changes
4. Ensure code follows the existing style and includes comments

For significant changes, please open an issue first to discuss.

## Roadmap

**MVP (Current)**
- Basic gesture detection (tap, swipe)
- Single-touch tracking
- Govee device control integration

**Future Considerations**
- Advanced gesture patterns (mult-finger taps and slides)
- Multi-device synchronization
- Mobile-based gesture configuration UI
- Additional smart device ecosystem support

## Support & Documentation

- **Bug Reports**: Use GitHub Issues in the relevant repository
- **Questions**: Check repository READMEs and inline code comments
- **Feature Requests**: Open a discussion in the organization

---

**Made with ⚡ for seamless gesture control**
