# Stone UPlugin Editor – User Documentation

## Overview
Stone UPlugin Editor is an Unreal Engine **editor-only plugin** that allows you to visually edit, validate, and manage `.uplugin` descriptor files without manually modifying JSON.  
It provides a structured UI, real-time validation, and clear feedback to ensure plugin descriptors remain valid and consistent.

---

## Opening the Editor
1. Launch Unreal Engine.
2. Open the **Plugins** window or use the menu entry added by Stone UPlugin Editor.
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

## Plugin Icon Requirements
- Icon size must be **128 × 128 pixels**
- Unsupported sizes trigger a validation warning or error
- Icon-related issues are clearly reported in the validation section

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

## Limitations
- Editor-only plugin
- No runtime impact
- Does not affect packaged builds
- Intended only for `.uplugin` descriptor management

---

## Uninstalling
1. Close Unreal Engine.
2. Remove the plugin folder from the project or engine `Plugins` directory.
3. Restart Unreal Engine.

---

## Versioning Notes
Always update version-related fields before distributing or publishing plugins to avoid conflicts or rejection.

---

## End of Documentation
