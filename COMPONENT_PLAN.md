# Component Plan — atc-security

This document details the components, primary data structures, and core functions implemented in `atc-security`.

## Core Component Specification

### 1. Security Audit (`audit/security_audit.atc`)
- **Module**: `security_audit`
- **ATC Standard**: `ATC-24`
- **Description**: Code scan, vulnerability detection, scoring
- **Key Data Structure**: `AuditScan`
- **Key Function**: `run_security_scan()` — Scans ATCLang codebase for security anti-patterns and vulnerabilities

### 1. Compliance Engine (`compliance/compliance_engine.atc`)
- **Module**: `compliance_engine`
- **ATC Standard**: `ATC-24`
- **Description**: Standard adherence, policy checks
- **Key Data Structure**: `ComplianceRule`
- **Key Function**: `check_compliance()` — Evaluates platform code against ATC security standards and regulations

### 1. Crypto Suite (`crypto/crypto_suite.atc`)
- **Module**: `crypto_suite`
- **ATC Standard**: `ATC-24`
- **Description**: SHA-256, ECDSA, AES, signature verification
- **Key Data Structure**: `CryptoKey`
- **Key Function**: `verify_signature()` — Verifies cryptographic signature using ECDSA or Ed25519

### 1. Threat Detection (`threats/threat_detector.atc`)
- **Module**: `threat_detector`
- **ATC Standard**: `ATC-24`
- **Description**: Anomaly, attack patterns, real-time alerts
- **Key Data Structure**: `ThreatAlert`
- **Key Function**: `detect_anomaly()` — Monitors real-time node logs and RPC traffic for attack vectors

### 1. Penetration Testing (`tests/penetration_test.atc`)
- **Module**: `penetration_test`
- **ATC Standard**: `ATC-24`
- **Description**: Automated attack simulation
- **Key Data Structure**: `PenTestConfig`
- **Key Function**: `simulate_attack()` — Runs automated adversarial attacks against network staging targets

### 1. Key Management (`keys/key_management.atc`)
- **Module**: `key_management`
- **ATC Standard**: `ATC-24`
- **Description**: Generation, rotation, HSM integration
- **Key Data Structure**: `KeyRing`
- **Key Function**: `rotate_key()` — Rotates active operational keypair and updates HSM configuration

