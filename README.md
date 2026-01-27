![DynamicSelector Logo](./Resources/repository-collaborators-icon.png)

# DynamicSelector
[Русская версия Readme](README.ru.md)

DynamicSelector is a Unity tool designed for creating
parametric selectors and filters based on external data.

The plugin allows you to configure filtering logic and parameter visualization
directly through the Unity Editor, without hardcoding logic and without
repeatedly implementing the same UI solutions manually.

---

## Key Features

- Creation of parametric selectors (filters, switches, ranges)
- Logic configuration via the Unity Editor
- Binding UI to external data sources
- Modular architecture with extensibility in mind
- Suitable for mobile, desktop, and web projects

---

## Who Is This Tool For

- **Unity developers** who need to implement filtering and parameter selection efficiently
- **Designers** working with UI and configurations without constant programmer involvement
- **Projects with dynamic data**, where parameter structures may change over time

---

## How It Works (Brief Overview)

1. A data structure is defined (XML feed)
2. A selector configuration is created in the Editor
3. Parameters are mapped to data fields
4. The UI automatically reacts to changes and filtering

---

## Requirements

- Unity 2021.3 LTS or newer  
- UI based on Unity UI / TextMeshPro  
- Project set to .NET Framework 4.x Equivalent

---

## Quick Start

Import the DynamicSelector package into your Unity project:

**Via Package Manager UI**
1. Open **Window → Package Manager**
2. Click **"+" → Add package from git URL...**
3. Enter: ```https://github.com/opodlinok/DynamicSelector.git?path=Packages/src```

**Or manually**
- Download the `.unitypackage` from the **Releases** section and import it into your project

**In the project**
1. Add the `FeedManager` component to a scene and configure its fields
2. Add the `FilterManager` component, assign it to `FeedManager`, and create filters as needed
3. Create an offer prefab with the `OfferView` component and assign it to `FeedManager`
4. Map data fields to UI parameters in `OfferView`
5. Run the scene and adjust the behavior

---

## Updates

The plugin includes a built-in update system  
(via **Toolbar → Window → DynamicSelector → Update Wizard**).

Manual updates are also available via the **Releases** section.

---

## Project Status

The project is under active development.

Planned for version 1.0.0:
- API stabilization
- Expanded documentation
- Support for additional data formats
- Improved Editor UX
- Sample scenes and a setup wizard

---

## Source Code

At the moment, DynamicSelector is distributed as compiled assemblies (.dll).

This repository is used for distributing releases, documentation,
and integration with Unity Package Manager.

Publishing the source code is not planned until the API is stabilized
and version 1.0 is released.

---

## Documentation

Detailed documentation, examples, and architectural notes
are available in the repository Wiki (in progress).

---

## License

See the [License.md](LICENSE.md) file for details.
