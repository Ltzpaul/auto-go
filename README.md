# Spruce Auto Farm — starter project

- Minecraft Java: 1.21.11
- Loader: Fabric
- Java: 21
- Mod ID: `spruceautofarm`
- Output name target: `SpruceAutoFarm.jar`

## Current state

This is a **starter prototype**, not the finished farming bot:
- Registers `K` to toggle the farm state.
- Registers `J` to toggle the order state.
- Displays a small HUD status panel.
- Does not yet plant, use Bone Meal, break blocks, move items, or interact with order menus.

## Build

Install JDK 21 and use Gradle 9.x. From this folder:

```bash
gradle build
```

The remapped mod JAR should appear in `build/libs/`.

## Important

Before implementing automated world interaction or automated order submission, check Hugo SMP's rules and obtain permission if macros/bots are restricted. Do not add anti-cheat bypasses, packet spoofing, or protection evasion.


## Build with GitHub Actions (recommended)

This project includes `.github/workflows/build.yml`. To build the mod on GitHub:

1. Create a new GitHub repository.
2. Extract this ZIP and upload the **contents of this project folder** to the repository root (so `.github` is directly at the root).
3. Open the repository's **Actions** tab. The workflow runs automatically after a push; you can also choose **Build Fabric Mod → Run workflow**.
4. Open the completed run and download the artifact named `SpruceAutoFarm-Minecraft-1.21.11`.
5. Inside the downloaded artifact is `SpruceAutoFarm.jar`.

The workflow uses Java 21 and Gradle 9.2.1, then uploads the remapped mod JAR. The sources JAR is not included in the artifact.
