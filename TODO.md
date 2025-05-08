# TODO: Verbesserungen basierend auf Terraform-Best-Practices

## 1. Code-Struktur
- [ ] **Module verwenden**: Prüfen Sie, ob alle gemeinsam genutzten Ressourcen in separaten Modulen organisiert sind.
- [ ] **Dateistruktur aufräumen**: Verschieben Sie gemeinsam genutzte Konfigurationsdateien wie `shared_variables.tf` in einen zentralen Ordner (`_shared` oder `modules`).
- [ ] **Outputs definieren**: Sicherstellen, dass alle wichtigen Ressourcen-Ausgaben (`outputs.tf`) definiert sind, um die Wiederverwendbarkeit zu verbessern.

## 2. Benennungskonventionen
- [ ] **Ressourcennamen**: Konsistente Benennung für Ressourcen (z. B. `vm-prod-app` statt `vm-${var.environment_prefix}-dc`).
- [ ] **Variablennamen**: Verwenden Sie beschreibende und konsistente Namen für Variablen, wie `vm_admin_password` statt `azure_vm_admin_password`.
- [ ] **Dateinamen**: Vermeiden Sie generische Namen wie `build.sh` oder `destroy.sh`. Verwenden Sie spezifische Namen wie `provision_resources.sh`.

## 3. Code-Styling
- [ ] **Kommentare hinzufügen**: Erläutern Sie komplexe Konfigurationsdetails in den `.tf`-Dateien.
- [ ] **Einrückung prüfen**: Stellen Sie sicher, dass die Einrückung in allen Dateien einheitlich ist (z. B. 2 Leerzeichen).
- [ ] **Formatierung**: Verwenden Sie `terraform fmt`, um alle `.tf`-Dateien automatisch zu formatieren.

## 4. Dokumentation
- [ ] **README aktualisieren**: Ergänzen Sie die README-Datei um klare Anweisungen zur Nutzung der Terraform-Dateien.
- [ ] **Variablen dokumentieren**: Erstellen Sie eine `variables.md`-Datei, die alle Variablen und deren Verwendung erklärt.

---

### Hinweise
Diese To-Do-Liste basiert auf den Empfehlungen von [Terraform Best Practices](https://www.terraform-best-practices.com/). Arbeiten Sie die Punkte schrittweise ab, um die Qualität und Wartbarkeit Ihres Codes zu verbessern.
