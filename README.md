# Nimbus

> [!NOTE]  
> This is a temporary fork to implement 24h time jankily. No PR because my code sucks :3

See the current temperature and weather conditions for your location with this minimal color-changing applet.

![Nimbus Screenshot](https://github.com/phynxinferno/nimbus-24h/blob/main/data/screenshot.png?raw=true)


## Building, Testing, and Installation

You'll need the following dependencies to build:
* libgeoclue-2-dev
* libgranite-7-dev >= 7.3.0
* libgtk-4-dev
* libgweather-4-dev
* meson
* valac

You'll need the following dependencies to run:
* geoclue-2.0

Run `flatpak-builder` to configure the build environment, download dependencies, build, and install

```bash
flatpak-builder build io.github.danirabbit.nimbus.json --user --install --force-clean --install-deps-from=appcenter
```

Then execute with

```bash
flatpak run io.github.danirabbit.nimbus
```
