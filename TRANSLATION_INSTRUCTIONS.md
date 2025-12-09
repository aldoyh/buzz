# Arabic translation & Tajawal font — instructions

This document explains how to integrate the provided Arabic locale and styles into the app.

1. Place the locale file
   - Add the Arabic translations to: `public/locales/ar.json`.

2. Load Tajawal font
   - Add the Google Fonts link for Tajawal into `public/index.html` `<head>`.

3. Add the RTL CSS
   - Add `src/styles/arabic.css` to the project and import/load it when Arabic is active.

4. Mark the document language and direction
   - When switching to Arabic, set `document.documentElement.lang = 'ar'` and `document.documentElement.dir = 'rtl'` or add a root class `lang-ar`.

5. Integrate with i18n
   - Add the `ar.json` file to your i18n setup and ensure the app uses translation keys.

6. Handle LTR content
   - Use a `.ltr` class for English/code snippets to preserve direction.

7. Flip layout where necessary
   - Manually adjust components that depend on left/right anchors.

8. Testing checklist
   - Verify layout, fonts, modals, icons and inputs in Arabic mode.
