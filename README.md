# vitrine-packs-starter

Starter-Beispielpakete fuer den [Vitrine](https://github.com/umgekocht/vitrine)-Katalog
(ROADMAP K8). Jeder Unterordner ist eine eigenstaendige Paketquelle im
`vitrine.json`-Format (siehe `registry/schema/vitrine.schema.json` im
Haupt-Repo), gebaut und signiert mit `cli/vitrine.js pack`/`sign` und als
`.vpkg`-Release-Asset an einem Tag dieses Repos veroeffentlicht.

## Pakete

| Ordner | Kategorie | Paket-ID |
|---|---|---|
| `mitternacht-theme/` | theme | `spassglas.mitternacht-theme` |
| `kompakt-hud/` | hud | `spassglas.kompakt-hud` |
| `steinbrocken-textur/` | texturen | `spassglas.steinbrocken-textur` |

Alle drei stehen unter `CC-BY-4.0`. Die Steinbrocken-Texturen sind bewusst
einfache, selbst erzeugte Platzhalter-Flaechen (kein Fremd-Asset,
Charter-Regel 6) -- ein handgezeichnetes Set ist in
`ASSETS-NEEDED.md` des Haupt-Repos als offen vermerkt.

## Releases

Jedes Paket hat einen eigenen Tag nach dem Muster `<ordner>-v<version>`
(z. B. `mitternacht-theme-v1.0.0`); das Release traegt das gebaute `.vpkg`
als Asset. Die Eintraege im Katalog (`vitrine-registry`,
`packages/<id>.json`) verweisen direkt auf diese Release-Assets.
