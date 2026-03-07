# REPLAYMAN-i18n

This repository contains the locale files for the **REPLAYMAN** frontend. These files enable the application to be translated into different languages, providing a localized experience for StarCraft II players all around the world.

## Repository Structure

All translation files are located in the `locales/` directory and use the **YAML** format (`.yml`). YAML allows us to include comments to provide context for translators.

- `locales/en.yml`: The source English translation file (reference for all keys and context).
- `locales/lorem.yml`: A placeholder file used for layout testing and UI development.
- `locales/[language-code].yml`: Additional language files (e.g., `es.yml`, `ko.yml`, `zh.yml`).

## YAML Tips for Translators

If you are new to YAML, here are a few important rules to keep your translation files valid:

### 1. Indentation is Critical
YAML uses spaces (not tabs) to define structure. 
- **Always use 2 spaces** per indentation level.
- Never use the Tab key; it will cause the application to crash.

### 2. Keys vs. Values
In a line like `welcome: Welcome to {name}.`:
- `welcome` is the **Key**: Do **NOT** change this. The application uses this ID to find the text.
- `Welcome to {name}.` is the **Value**: This is what you should translate.

### 3. Handling Special Characters & Quotes
Most of the time, you don't need quotes. However, use them if your translation starts with a special character or contains a colon:
- **Single quotes** (`'`) are generally preferred: `title: 'StarCraft: Legacy of the Void'`
- If your translation contains a single quote (apostrophe), wrap the whole thing in **double quotes** (`"`) or double the single quote:
  - `glad: "We're glad you're here."`
  - `glad: 'We''re glad you''re here.'`

### 4. Multi-line Translations
For very long paragraphs, you can use the pipe character (`|`) to keep the formatting clean:
```yaml
description: |
  This is a very long
  paragraph that spans
  multiple lines in the file.
```

## How to Contribute

We welcome contributions to improve our existing translations or to add support for new languages! Here is how you can help:

### 1. Editing an Existing Translation

If you find a typo, a grammatical error, or a better way to phrase something:

1.  Navigate to the `locales/` directory.
2.  Locate the YAML file for the language you want to edit.
3.  Modify the values corresponding to the keys you wish to update. **Refer to the comments in `en.yml` if you need more context on how a string is used in the app.**
4.  Commit your changes and open a **Pull Request**.

### 2. Adding a New Translation

To add support for a completely new language:

1.  Copy the `locales/en.yml` file.
2.  Rename the copy using the appropriate ISO 639-1 language code (e.g., `ko.yml` for Korean, `zh.yml` for Chinese).
3.  Translate the values in the new file while keeping the keys exactly the same. **Please keep the comments intact**, as they help future contributors understand the purpose of each string.
4.  Commit your new file and open a **Pull Request**.

## Guidelines for Translators

- **Preserve Placeholders**: Many strings contain placeholders like `{name}`, `{theme}`, or `{version}`. Do **not** translate these placeholders.
- **Respect Comments**: Use the comments in `en.yml` to understand the technical context (e.g., whether a string is a button, a tooltip, or a header).
- **Consistency**: Try to maintain consistent terminology throughout the translation.

## Reporting Issues

If you notice a translation issue but cannot fix it yourself, please report it on our [Issues](https://github.com/stegoresearch/REPLAYMAN-i18n/issues) page.

## License

This project is licensed under the Apache License, Version 2.0. See the `LICENSE` file for more details.
