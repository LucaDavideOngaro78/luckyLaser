# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

### Added
- Add support to skip setting buffer omnifunc (#1079).
- Add support of setting languageclient binary path (#1020).
- Support file watching scenario of writing via rename (#1054).

## [0.1.158]

### Added
- Add support of multiple configuration files (#1013).
- Add support for code actions using ranges.
- Add support of `$/progress` notification.
- Use a minimal style for neovim's floating window and add support for override (#1033).
- Add `hideVirtualTextsOnInsert` option (#982).
- Add support of populating `source` in diagnostics (#1062).
- Add support of overriding selection UI (#1059, #1060).
- Add plug mappings (#1065).

### Changed
- Hide error of `ContentModified` (#997).
- Do not show `window/logMessage` messages (#1056).
- Change aarch64 build from `-gnu` to `-musl` (#1044).

### Fixed
- Fix issue of no signs in sign column and virtual text on Windows (#970).
- Fix error handling of install script (#1011).
- Fix detection of Haskell cabal project root (#1048).
- Fix rust-analyzer runnable actions (#1058).

### Thanks
Huge thanks to Martin (@martskins) for numerous contributions to this release,
from improving overall code structure, addressing pain points to answering
issues.

## [0.1.157]

### Added

- Update cursor location properly after additional text edits (like automatic import) applied in completion (#961)
- Add [CHANGELOG](https://github.com/autozimu/LanguageClient-neovim/blob/next/CHANGELOG.md).
- Add support for `rust-anaylzer.selectAndApplySourceChange` (#965)
- Add support to customize highlight for floating hover window (#966)
- Add support for the proposed semantic highlighting (#954)
- Add `LanguageClient_applyCompletionAdditionalTextEdits` flag (#978)
- Add default root path for Go project (#976)
- Add doc for installation on ArchLinux through aur (#988)
- Add CodeLens integration with FZF (#996)
- Add option to set preferred MarkupKind (#972)
- New function `LanguageClient#isServerRunning()` for statusline integration (#1003)
- New function `LanguageClient#statusLineDiagnosticsCounts` (#1006)

### Fixed

- Fix issue calling `nvim_create_namespace` under vim #967
- Fix signs not cleanup #1008
