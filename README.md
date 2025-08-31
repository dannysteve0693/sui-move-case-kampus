# Kampus Move Package

This Move package provides smart contract modules for managing university (kampus) data on-chain. It demonstrates various Move features and patterns for handling student records, capabilities, and shared/owned objects.

## Features

- **Mahasiswa Data Management**
  - Store detailed student profiles: name, NIM, major, age, credits (SKS), status (active/graduated).
  - Functions for registering students, updating SKS, graduation status, and more.

- **Boolean, Number, String, and Vector Examples**
  - [`belajar_boolean.move`](sources/belajar_boolean.move): Manage student status with booleans.
  - [`belajar_number.move`](sources/belajar_number.move): Handle numeric student data (NIM, age, SKS).
  - [`belajar_string.move`](sources/belajar_string.move): Work with student names using strings.
  - [`belajar_vector.move`](sources/belajar_vector.move): Store lists of student names and NIMs.

- **Capabilities Pattern**
  - [`capabilities_pattern.move`](sources/capabilities_pattern.move): Demonstrates admin/dosen capabilities for access control.

- **Shared and Owned Objects**
  - [`shared_objects.move`](sources/shared_objects.move): Shared campus registry accessible by all.
  - [`owned_objects.move`](sources/owned_objects.move): Owned student cards, transferable between users.

- **Comprehensive Functions**
  - [`fungsi_lengkap.move`](sources/fungsi_lengkap.move): Full-featured student profile creation with validation and error handling.

- **Main Kampus Module**
  - [`kampus.move`](sources/kampus.move): Central logic for campus registry, student profiles, events, and view functions.

## Getting Started

1. Install [Sui Move CLI](https://docs.sui.io/build/install).
2. Clone this repo and enter the `kampus` directory.
3. Build the package:
   ```sh
   sui move build
   ```
4. Run tests:
   ```sh
   sui move test
   ```

## Folder Structure

- `sources/` - Move source files (modules).
- `tests/` - Move unit tests.
- `build/` - Compiled bytecode and debug