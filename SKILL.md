---
name: flux-ui
description: Use when building, modifying, reviewing, or debugging user interfaces that use Laravel Flux UI components. Trigger for Flux component usage, props, variants, layouts, forms, tables, modals, menus, navigation, and Flux-specific styling. Do not trigger for generic Laravel backend work, Eloquent models, migrations, queues, APIs, or Blade views that do not use Flux.
---

# Flux UI

Use the project's installed Flux version as the source of truth.

Before using unfamiliar Flux APIs:
- Check the installed Flux and Livewire versions.
- Prefer official Flux components over custom Blade implementations.
- Consult the official Flux Markdown documentation when component syntax, props, slots, or behavior are uncertain.
- Do not invent undocumented Flux APIs.
- Check whether Flux Pro is installed before using Pro-only components.

# Flux Pro

If Flux Pro availability cannot be determined and a Pro-only component or feature is relevant, ask the user:

"Do you have Flux Pro installed in this project?"

## Documentation

Flux provides AI-ready official documentation.

Before using unfamiliar Flux components or APIs:

1. Check the installed Flux version.
2. Consult:
   https://fluxui.dev/llms.txt
3. Prefer Markdown component documentation:
   https://fluxui.dev/components/{component}.md
4. Do not infer undocumented props, slots, variants, or behavior.
5. When necessary, inspect the official source:
   https://github.com/livewire/flux