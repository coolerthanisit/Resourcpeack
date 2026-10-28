# CataclysmEngine downloads

Target: **Paper 1.21.11**, **Java 25**, vanilla Minecraft Java 1.21.11 clients.

- [Download plugin JAR](CataclysmEngine.jar?raw=true)
- [Download resource pack ZIP](CataclysmEngine-ResourcePack.zip?raw=true)
- [Download complete source ZIP](CataclysmEngine-Source.zip?raw=true)
- [Resource-pack SHA-1](CataclysmEngine-ResourcePack.sha1)
- [Artifact checksums](MANIFEST.json)

## Installation

1. Put `CataclysmEngine.jar` in your Paper 1.21.11 test server's `plugins` folder. Run the server with Java 25.
2. Host the resource-pack ZIP at an HTTPS direct-download URL. Keep the pack zipped.
3. Set `resource-pack.url` and `resource-pack.sha1` in `plugins/CataclysmEngine/config.yml`. The SHA-1 is `19363314dbb1aa8b619ccd74f439fefc80dba3e6`.
4. Run `/disaster reload`, then `/disaster pack send`, and accept the pack. As an operator outside spawn protection, try `/disaster gui` or `/disaster preview meteor`.

Destruction defaults to VISUAL_ONLY, damage is disabled, and automatic disasters are disabled. The source archive includes the complete installation guide, specification coverage report, build scripts, source code, assets, and test results.

## Verification and limitations

The Java 25 Gradle build compiled against official pinned Paper 1.21.11 API sources through the documented source composite fallback. All 19 distinct JUnit tests passed. Resource-pack JSON, model and texture references, animations, PNGs, OGG decoding, ZIP layout and checksums passed structural checks.

**Actual Paper server startup, Minecraft client rendering/audio, multiplayer load, protection integration and crash recovery acceptance tests remain unrun.** Official Paper download hosts were blocked by the development environment's network policy. This is an implemented project with documented specification gaps, not a fully validated premium release. Read `docs/REQUIREMENTS.md` and `docs/TEST_RESULTS.md` inside the source archive before production use.
