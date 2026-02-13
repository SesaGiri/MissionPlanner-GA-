# Garuda Ops Control (Indigenous Edition)

Garuda Ops Control is a privately branded ground-control application customized from this codebase to present an indigenous drone operations experience inspired by the style and tone of Garuda Aerospace.

## What changed in this customization

- Product branding renamed to **Garuda Ops Control**.
- Splash/title messaging updated for an indigenous operations identity.
- Vendor shortcut/menu link routed to Garuda Aerospace website.
- Local data/log folders and app metadata updated to remove Mission Planner naming in primary app settings.

## Build in Visual Studio

1. Install Visual Studio 2022 with `.NET desktop development` workload.
2. Open `MissionPlanner.sln`.
3. Set startup project to `MissionPlanner`.
4. Build using **Build > Build Solution**.
5. Run with **F5**.

## Build & run from VS Code

### Prerequisites

- .NET SDK 8+
- C# Dev Kit extension (recommended)

### CLI workflow

```bash
dotnet restore MissionPlanner.csproj
dotnet build MissionPlanner.csproj -c Debug
dotnet run --project MissionPlanner.csproj
```

### Debug workflow in VS Code

1. Open folder in VS Code.
2. Run **.NET: Generate Assets for Build and Debug**.
3. Select `MissionPlanner.csproj` when prompted.
4. Press **F5** to start debugging.

## Personal deployment notes

- Place custom assets in app run directory:
  - `logo.txt` (first line used as app display name)
  - `logo.png` (main title/logo)
  - `logo2.png` (header branding strip)
  - `icon.png` (app icon)
  - `splashbg.png` (splash background)
- Package with your preferred installer or zip deployment.

## Legal note

This repository contains upstream open-source components. If you redistribute, review license obligations in `COPYING.txt`.
