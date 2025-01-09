# XMRig

**XMRig** is a high-performance, cross-platform CPU and GPU miner designed for mining various cryptocurrencies, primarily focusing on the **Monero (XMR)** cryptocurrency, which uses the **RandomX** hashing algorithm. The software is open-source and is widely regarded for its efficiency, configurability, and active development.

## Key Features

- **Support for Multiple Algorithms**  
    XMRig supports a variety of hashing algorithms, including:
    
    - **RandomX** (primarily for Monero)
    - **CryptoNight** (variants like CryptoNight-lite, CryptoNight-heavy)
    - **Argon2** (used by some altcoins)
- **CPU and GPU Mining**  
    XMRig allows users to mine using:
    
    - **CPUs** (optimized for modern architectures, including support for AES-NI and AVX)
    - **GPUs** (support for NVIDIA and AMD cards)
- **Cross-Platform Compatibility**  
    Compatible with major operating systems:
    
    - **Windows**
    - **Linux**
    - **macOS**
    - **FreeBSD**
- **Optimized Performance**
    
    - Highly optimized for low-power consumption and maximum hash rate.
    - Advanced tuning options, including thread and affinity management.
- **User-Friendly Configuration**
    
    - JSON-based configuration files.
    - Command-line options for quick customization.
    - Built-in benchmarking and performance statistics.
- **Advanced Features**
    
    - **Remote management:** API for monitoring and controlling the miner.
    - **Low-level optimizations:** Uses assembly language for critical operations.
    - **Dynamic algorithm switching:** Adapts to changing network conditions or mining needs.

## Getting Started

### Prerequisites

Before you begin, ensure your system meets the following requirements:

- **Modern CPU** with at least SSE2 support.
- **Supported GPU** (if GPU mining):
    - NVIDIA: CUDA Toolkit installed.
    - AMD: OpenCL runtime installed.
- **64-bit operating system** for optimal performance.

### Installation

1. **Download the precompiled binaries** from the [Releases](https://github.com/xmrig/xmrig/releases) page.
2. Alternatively, **build from source**:
    
    bash
    
    Копировать код
    
    `git clone https://github.com/xmrig/xmrig.git cd xmrig mkdir build cd build cmake .. make`
    

### Configuration

XMRig can be configured via:

- **Command-line arguments**  
    Example:
    
    bash
    
    Копировать код
    
    `xmrig -o pool.example.com:3333 -u wallet_address -p x`
    
- **Config.json file**  
    Edit the `config.json` file for more granular settings, such as:
    - Pool settings
    - Algorithm preferences
    - Thread management

### Running the Miner

To start mining, simply run:

bash

Копировать код

`xmrig`

Monitor the output for real-time performance metrics, such as hash rate and accepted shares.

## Donation Program

By default, XMRig includes a small developer fee (1%) to support ongoing development. This can be modified or disabled by recompiling the source code. However, supporting the developers is highly encouraged to ensure the project’s sustainability.

## Security and Privacy

- XMRig is designed to prioritize user privacy. It does not collect or transmit personal data.
- Ensure you download XMRig from official sources to avoid malicious versions.

## Community and Support

XMRig has an active and supportive community. For help, updates, or discussions:

- Visit the [official website](https://xmrig.com).
- Join the [GitHub Discussions](https://github.com/xmrig/xmrig/discussions) or report issues in the [Issues Tracker](https://github.com/xmrig/xmrig/issues).
- Engage with the community on platforms like Reddit or dedicated cryptocurrency forums.

## Contributing

Contributions are welcome! Whether it’s reporting bugs, submitting feature requests, or improving documentation, feel free to open a pull request or issue.

## License

XMRig is licensed under the **GPL-3.0** license, ensuring that the software remains free and open for everyone to use, modify, and distribute.
