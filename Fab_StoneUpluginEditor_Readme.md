# Stone UPlugin Editor – User Documentation

## Overview
Stone UPlugin Editor is an Unreal Engine **editor-only plugin** that allows you to visually edit, validate, and manage `.uplugin` descriptor files without manually modifying JSON.  
It provides a structured UI, real-time validation, and clear feedback to ensure plugin descriptors remain valid and consistent.

---

## Setup the plugin
Install it through Fab/EpicGames launcher.
or
Copy plugin folder and past it in your project's Plugins folder.

Enable plugin through plugins widow in unreal engine.

---
<img width="534" height="231" alt="OpenEditor_window" src="https://github.com/user-attachments/assets/c826ea4c-03cf-4229-9a27-97c14697d3fa" />

## Opening the Editor
1. Launch Unreal Engine.
2. Open the windows menu and click on the menu entry added by Stone UPlugin Editor under section `Stone Ecosystem`.
3. Select the plugin you want to edit.
4. The plugin’s `.uplugin` descriptor opens in the custom editor UI.

---

## Editor Layout
The editor is divided into logical sections that mirror the plugin descriptor structure:
- Plugin Metadata
- Versioning Information
- Modules
- Dependencies
- Platform Settings
- Icon & Resources
- Validation Summary

Each section updates the descriptor immediately when values change.

---

## Editing a Plugin Descriptor
- Modify fields directly in the editor UI.
- Changes are applied instantly to the descriptor.
- No manual JSON editing is required.
- Save the plugin as usual to persist changes.

---

## Validation System
- Validation runs automatically whenever a field changes.
- Errors and warnings are shown in the **Validation Summary** section.
- Each section validates only its relevant data.
- If no errors or warnings exist, the validation section collapses automatically.

### Common Validations
- Missing required fields
- Invalid version values
- Incorrect module definitions
- Missing or invalid plugin icon
- Icon size validation (128×128)

---

## Fixing Validation Errors
1. Open the **Validation Summary** section.
2. Review listed errors or warnings.
3. Navigate to the related editor section.
4. Correct the issue.
5. Validation updates automatically.

---

## Best Practices
- Always use the editor instead of manually editing `.uplugin` JSON files
- Resolve warnings before packaging or distributing plugins
- Keep plugin metadata complete and accurate
- Validate icons before final submission

---

## Support and feedback
Email : stonesparkstudio@gmail.com
