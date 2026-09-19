# Record Override Detector — Community INI List

This repository maintains the community configuration for `RecordOverrideDetector.ini`.

Contributions are welcome for:

```ini
[ExcludedPlugins]
Unofficial Fallout 4 Patch.esp
PPF.esm
PRP.esp

[OverridePermitted]
CBBEHolyFix.esp > CBBE.esp
```

Use `[ExcludedPlugins]` only for plugins that should be ignored globally by the detector.

Use `[OverridePermitted]` for known, intentional override relationships where the plugin on the left is expected to take precedence over the plugin on the right.

Format:

`WinningPlugin.esp > OverriddenPlugin.esp`

Before submitting a change:

* Use the exact plugin filename.
* Keep entries case-consistent with the actual file when possible.
* Add only well-known or verified intentional relationships.
* Do not add speculative compatibility rules.
* Avoid duplicate entries.
* Keep the file clean and one entry per line.

Pull requests should briefly explain why the exclusion or permitted override is intentional.
