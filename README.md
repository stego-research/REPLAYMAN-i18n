# REPLAYMAN-i18n

This repository contains the locale files for the **REPLAYMAN** frontend. These files enable the application to be translated into different languages, providing a localized experience for lovers of StarCraft II all around the world.

## Repository Structure

All translation files are located in the `locales/` directory:

- `locales/en.json`: The source English translation file (reference for all keys).
- `locales/lorem.json`: A placeholder file used for layout testing. This can help you understand 
- `locales/[language-code].json`: Additional language files (e.g., `es.json`, `ko.json`, `zh.json`).

## How to Contribute

We welcome contributions to improve our existing translations or to add support for new languages! We believe strongly in the global scene and would love to have your help. Here is some information on how you can contribute.

### 1. Editing an Existing Translation

If you find a typo, a grammatical error, or a better way to phrase something in an existing language file:

1.  Navigate to the `locales/` directory.
2.  Locate the JSON file for the language you want to edit.
3.  Modify the values corresponding to the keys you wish to update.
4.  Commit your changes and open a **Pull Request**.

### 2. Adding a New Translation

To add support for a completely new language:

1.  Copy the `locales/en.json` file.
2.  Rename the copy using the appropriate ISO 639-1 language code (e.g., `ko.json` for Korean, `zh.json` for Chinese).
3.  Translate the values in the new file while keeping the keys exactly the same.
4.  Commit your new file and open a **Pull Request**.

## Guidelines for Translators

- **Preserve Placeholders**: Many strings contain placeholders like `{name}`, `{theme}`, or `{version}`. Do **not** translate these placeholders, as they are dynamically replaced by the application.
- **Maintain JSON Structure**: Ensure the JSON structure remains valid (correct usage of quotes, commas, and braces).
- **Consistency**: Try to maintain consistent terminology throughout the translation.

## Reporting Issues

If you notice a translation issue but cannot fix it yourself, please report it on our [Issues](https://github.com/stegoresearch/REPLAYMAN-i18n/issues) page.

When reporting an issue, please include:
- The language file affected.
- The specific key or text that needs attention.
- A suggested correction if possible.

## License

This project is licensed under the Apache License, Version 2.0. See the `LICENSE` file for more details.
