# Changelog

## [0.3.0-2]

### Added

- Added versioning support for kvm bindings structures used
  in VM serialization on arm and arm64.

## [0.3.0-1]

### Added

- [upstream] Enabled `fam-wrappers` support on arm and arm64.
- [upstream] Added fam-wrapper for the arm specific `kvm_reg_list` struct.

## [0.2.0-2]

### Changed

- Updated to `versionize` from crates.io.

## [0.2.0-1]

Built on top of upstream rust-vmm/kvm-bindings v0.2.0.

### Added

- Added versioning support for kvm bindings structures used
  in VM serialization on x86_64.

## [0.2.0]

### Added

- Added opt-in feature `fam-wrappers` that enables exporting
  safe wrappers over generated structs with flexible array
  members. This optional feature has an external dependency
  on `vmm-sys-util`.
- Added safe fam-wrappers for `kvm_msr_list`, `kvm_msrs`,
  and `kvm_cpuid2`.

## [0.1.1]

### Changed

- Do not enforce rust Edition 2018.

## [0.1.0]

### Added

- KVM bindings for Linux kernel version 4.14 and 4.20 with
  support for arm, arm64, x86 and x86_64.
