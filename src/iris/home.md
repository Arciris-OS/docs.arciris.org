# Iris Package Manager

This section contains comprehensive documentation for the Iris package manager.

> **Note:** If you're looking for documentation about the noa init system, please refer to [noa's documentation](../noa/home.md).

## Overview

Iris is a modern package manager designed for system-level package management with a focus on security, reliability, and automated dependency resolution. It provides a streamlined approach to software installation and maintenance while ensuring system integrity through comprehensive verification processes.

## Key Features

Iris offers the following core capabilities:

### 1. Package Installation
- **Automated Installation**: Seamlessly install packages from configured repositories
- **Multi-source Support**: Install packages from various sources including local files and remote repositories
- **Version Management**: Support for specific version installation and version constraints
- **Installation Verification**: Real-time verification during the installation process

### 2. Package Removal
- **Clean Uninstallation**: Complete removal of packages including associated files and configurations
- **Dependency-aware Removal**: Intelligent removal that considers dependent packages
- **Rollback Support**: Ability to restore previously removed packages when needed
- **Orphaned Package Cleanup**: Automatic detection and removal of unused dependencies

### 3. Automatic Dependency Resolution
- **Smart Dependency Solver**: Automatically resolves and installs required dependencies
- **Conflict Detection**: Identifies and resolves package conflicts before installation
- **Circular Dependency Handling**: Advanced algorithms to handle complex dependency chains
- **Version Compatibility**: Ensures compatibility between dependent packages and their versions

### 4. Boot-time Checksum Validation
- **Integrity Verification**: Automatically verifies package checksums during system boot
- **Corruption Detection**: Identifies corrupted packages that may compromise system stability
- **Performance Optimized**: Fast checksum verification that doesn't significantly impact boot time
- **Error Reporting**: Clear reporting of checksum failures with suggested remediation steps

### 5. Cryptographic Package Integrity
- **Minisign Integration**: Uses minisign for cryptographic verification of package authenticity
- **Tamper Detection**: Ensures packages haven't been modified since signing
- **Publisher Verification**: Validates that packages come from trusted sources
- **Signature Chain Validation**: Comprehensive verification of the entire signature chain

### 6. Stage1 Package Validation
- **Critical System Components**: Special validation for Stage1 packages essential for system boot
- **Boot Safety**: Ensures critical packages are intact before system initialization
- **Emergency Recovery**: Built-in mechanisms to handle Stage1 package corruption
- **Priority Validation**: Fast-track verification for essential system components

## Security Model

Security is a fundamental aspect of Iris design:

- **Cryptographic Signatures**: All packages must be cryptographically signed
- **Trusted Publishers**: Configurable trust model for package publishers
- **Integrity Monitoring**: Continuous monitoring of installed package integrity
- **Secure Bootstrap**: Verification starts from the earliest boot stages

## Getting Started

To begin using Iris, refer to the installation guide and configuration documentation in the following sections.

## Related Documentation

- [Installation Guide](installation.md) - How to install and configure Iris
- [Configuration Reference](configuration.md) - Detailed configuration options
- [Command Reference](commands.md) - Complete command-line interface documentation
- [Repository Management](repositories.md) - Managing package repositories
- [Security Configuration](security.md) - Advanced security settings
- [Troubleshooting](troubleshooting.md) - Common issues and solutions






