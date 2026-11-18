# Contributing

Thanks for helping bring Flutter apps to older LG webOS TVs.

## Most useful right now

1. **TV compatibility reports** from any webOS release other than 6. Use the
   [TV compatibility report](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos/issues/new?template=tv_compat_report.yml)
   form; the test apps in `legacy-webos/tests` produce the results it asks for.
2. **Bug reports** with a minimal app and `compat.log`.
3. **Fixes** for the open items in `legacy-webos/README.md` (known issues) and the porting guide.

## Where things go

| Change | Repository |
| --- | --- |
| Packager, shims, `--legacy`, tools, test apps | [flutter-webos](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos), under `legacy-webos/` |
| `flutter-webos` CLI | [flutter-webos](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos) |
| A plugin | [plugins](https://github.com/Webos-Flutter-Legacy-TV/plugins), under `packages/<plugin>/` |
| Website | [webos-flutter-legacy-tv.github.io](https://github.com/Webos-Flutter-Legacy-TV/webos-flutter-legacy-tv.github.io) |
| Issue/PR templates, this file | [.github](https://github.com/Webos-Flutter-Legacy-TV/.github) |

Problems that also happen with LG's unmodified SDK on webOS 26 belong
[upstream](https://github.com/lg-flutter-webos).

## Getting set up

Follow **Setup** in
[legacy-webos/README.md](https://github.com/Webos-Flutter-Legacy-TV/flutter-webos/blob/main/legacy-webos/README.md#setup)
(Linux x86_64 host). `setup.sh` downloads everything into git-ignored folders;
nothing is installed system-wide.

## Pull requests

- Branch from `main`, keep each pull request to one topic, and fill in the template.
- Write commit messages that say **why** the change is needed.
- Say exactly what you tested and on which TV and release. If you couldn't test
  on a TV, say so; someone with hardware can pick it up.
- New behaviour in the shims that hasn't been verified on real TVs should be
  **opt-in** (an empty switch file in `webos/meta/`, like the existing
  `compat-*` switches) until it has been.
- Update the docs when behaviour changes.

## Licences

Most code is BSD-3-Clause, as LG released it. Some LG files carry other
terms (for example `SPDX-License-Identifier: LicenseRef-LGE-Proprietary` in a
few plugins); each file's header says which applies, and third-party notices
are in each repo's `LICENSES/`. Keep existing headers as they are. New files
use BSD-3-Clause, and contributions are accepted under it.

- **Don't copy code from GPL-licensed projects** into these repositories, even
  small parts. Reading them for ideas is fine; write your own implementation.
- Keep licence headers on third-party code you add, and list it in the repo's
  licence notices.

## Privacy

Never commit or paste personal data: TV IP addresses, serial numbers, MAC
addresses, account names, tokens or keys. Check logs and survey output before
attaching them.

## Conduct

Everyone taking part follows the [Code of Conduct](CODE_OF_CONDUCT.md).
