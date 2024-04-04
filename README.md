<p align="center">
    <img src="https://raw.githubusercontent.com/nunomaduro/pint-strict-preset/main/art/banner.png" width="600" alt="Pint Strict Preset">
</p>

------

Pint strict preset is an insanely defensive coding style preset for those who demand meticulous precision in their projects. To use it, simply create a `pint.json` file with the following contents:

```json
{
    "preset": "laravel",
    "exclude": [
        "vendor/"
    ],
    "rules": {
        "array_push": true,
        "backtick_to_shell_exec": true,
        "declare_strict_types": true,
        "fully_qualified_strict_types": true,
        "global_namespace_import": {
            "import_classes": true,
            "import_constants": true,
            "import_functions": true
        },
        "ordered_imports": {
            "sort_algorithm": "length",
            "imports_order": [
                "const",
                "class",
                "function"
            ]
        },
        "ordered_class_elements": {
            "order": [
                "use_trait",
                "case",
                "constant",
                "constant_public",
                "constant_protected",
                "constant_private",
                "property_public",
                "property_protected",
                "property_private",
                "construct",
                "destruct",
                "magic",
                "phpunit",
                "method_abstract",
                "method_public_static",
                "method_public",
                "method_protected_static",
                "method_protected",
                "method_private_static",
                "method_private"
            ],
            "sort_algorithm": "none"
        },
        "ordered_interfaces": true,
        "ordered_traits": true,
        "protected_to_private": true,
        "strict_comparison": true
    }
}
```
