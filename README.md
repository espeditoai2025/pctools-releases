# PcTools — download

Questo repository contiene solo i pacchetti di installazione di **PcTools**, l'app per Windows 11 di
diagnosi e riparazioni guidate sviluppata da PCS di Ambrosio Espedito. Il codice sorgente non è pubblico.

Sito: https://pctools.it

## Versioni

| Versione | Tipo | Requisiti |
| --- | --- | --- |
| [0.2.0-dev](https://github.com/espeditoai2025/pctools-releases/releases/tag/v0.2.0-dev) | Sviluppo, per il collaudo — **consigliata** | Windows 11 a 64 bit |
| [0.1.0-dev](https://github.com/espeditoai2025/pctools-releases/releases/tag/v0.1.0-dev) | Sviluppo, superata (mostra un errore durante la diagnosi) | Windows 11 a 64 bit |

## Prima di installare una versione di sviluppo

- **Non è firmata digitalmente**: Windows SmartScreen può segnalare un editore sconosciuto.
- **Non è ancora collaudata** su macchine virtuali e PC reali: non installarla sui PC dei clienti.
- Scaricala solo da https://pctools.it o da questa pagina e **verifica l'hash SHA-256** pubblicato
  nelle note della versione. In PowerShell, nella cartella del file:

```powershell
Get-FileHash .\PcTools-Setup-0.2.0-dev-win-x64.exe -Algorithm SHA256
```

## Cosa installa

PcTools viene installato in `Programmi\PcTools` (serve l'autorizzazione di amministratore solo per
l'installazione) e si disinstalla dalle impostazioni di Windows. I rapporti e i log locali restano in
`%LOCALAPPDATA%\PcTools`. Il programma non invia telemetria. Gli avvisi sui componenti di terze parti
sono nel file `THIRD-PARTY-NOTICES.md` della cartella di installazione.

© 2026 PCS di Ambrosio Espedito. Tutti i diritti riservati.
