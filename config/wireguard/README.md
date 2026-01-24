Anleitung für `linuxserver/wireguard` config

- Dieser Ordner wird vom Container unter `/config` verwendet.
- Beim ersten Start erstellt der Container die WireGuard-Konfiguration hier (z. B. `peer1/peer1.conf`).
- Passen Sie `SERVERURL` in `docker-compose.yml` an Ihre öffentliche IP oder Ihren Hostnamen an.
- Falls SELinux/AppArmor aktiv ist, prüfen Sie Rechte/Policies.

Starten:

```powershell
docker compose up -d
```

Logs anschauen:

```powershell
docker compose logs -f wireguard
```
