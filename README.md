# Northstar Commerce — installere

Dette repoet distribuerer ferdige Windows-installere og oppdateringsmanifest.
Kildekoden ligger i et separat, privat repo og publiseres ikke her.

## Last ned

Åpne [utgivelser](https://github.com/ArneRiseth/webshop1-releases/releases) og last
ned installeren for ønsket versjon. Utgivelser merket `experimental` er
forhåndsutgivelser for testing.

## Oppgradering

Vanlig oppgradering med installer er fortsatt støttet: kjør som administrator
på Windows-serveren og velg den eksisterende nettbutikken som skal oppgraderes.

Fra **2.0.150** kan administratoren aktivere oppgradering under **System og
 tilgang → Oppgradering av nettbutikk**. Se etter ny versjon og bekreft planlagt
midlertidig driftsstans før oppgraderingen startes. Ingen GitHub-nøkkel eller
GitHub-konto er nødvendig på kundeinstallasjonen.

Versjon 2.0.150 må installeres manuelt én gang for å bytte eldre installasjoner
til dette offentlige distribusjonsrepoet. Oppgraderingsagenten tar en lokal
sikkerhetskopi og kontrollerer ny oppstart. Alvorlige feil holder butikken på
pause for manuell gjenoppretting; automatisk tilbakeføring er ikke implementert.

## Innhold i en utgivelse

- `NorthstarCommerce-<versjon>[-experimental]-win-x64.exe`: installer.
- `northstar-update.json`: versjon, kanal, filstørrelse og SHA-256.

Installeren og manifestet er offentlig tilgjengelige. Repoets automatisk
opprettede kildearkiver inneholder bare dette distribusjonsrepoets README og
historikk, ikke applikasjonens kildekode. Installerne er foreløpig ikke
Authenticode-signert. En ekte oppgradering av en registrert Windows-tjeneste
med administratorrettigheter er ennå ikke verifisert i utviklingsmiljøet.