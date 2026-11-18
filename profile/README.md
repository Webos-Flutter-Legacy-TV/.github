## Flutter apps on older LG webOS TVs

LG's Flutter SDK for webOS ([lg-flutter-webos](https://github.com/lg-flutter-webos))
builds apps for **webOS 26** only. This organisation keeps forks of those
repositories with the changes needed to run the same apps on **older webOS TV
releases**, starting with webOS 6.

**Website:** https://webos-flutter-legacy-tv.github.io

| Repository | What it holds |
| --- | --- |
| [flutter-webos](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos) | The `flutter-webos` CLI plus [`legacy-webos/`](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos/tree/main/legacy-webos): the packager, compatibility shims, tools, test apps and the [porting guide](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos/blob/main/legacy-webos/docs/PORTING-GUIDE.md) |
| [plugins](https://github.com/Webos-Flutter-Legacy-TV/plugins) | webOS plugins with fixes found while porting (video_player, audioplayers_soloud, flutter_secure_storage, ...) |
| [ndk](https://github.com/Webos-Flutter-Legacy-TV/ndk), [artifacts](https://github.com/Webos-Flutter-Legacy-TV/artifacts), [devcontainer](https://github.com/Webos-Flutter-Legacy-TV/devcontainer), [plugins-beta](https://github.com/Webos-Flutter-Legacy-TV/plugins-beta) | Forks kept in step with upstream |

### Status

| webOS | Status |
| --- | --- |
| 26 | LG's own target |
| 22-25 | Expected to work (firmware check passes; not run on a TV yet) |
| 6 | **Verified** on webOS 6.5.3: UI, remote, networking, storage, video, audio, PlayReady, opt-in Widevine |
| 5 | Likely works (one media function shimmed) |
| 4 and older | Needs more work |

### Get involved

- Own a webOS TV that isn't webOS 6? A **[TV compatibility report](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos/issues/new?template=tv_compat_report.yml)** is the most useful thing you can send.
- Found a bug? [Open an issue](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos/issues/new/choose).
- Read [CONTRIBUTING](https://github.com/Webos-Flutter-Legacy-TV/.github/blob/main/CONTRIBUTING.md) before sending a pull request.

<sub>Community project, not affiliated with or endorsed by LG Electronics. webOS and LG are trademarks of LG Electronics.</sub>
