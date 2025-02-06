# keycloak
Keycloak – Open-Source-Identity- und Access-Management

Keycloak ist eine leistungsstarke Open-Source-Lösung für Identity- und Access-Management (IAM). Die Software ermöglicht es, Benutzerverwaltung, Authentifizierung und Autorisierung für Anwendungen und Dienste zentral zu steuern. Als Open-Source-Projekt der Red Hat Community bietet Keycloak eine flexible und skalierbare Alternative zu proprietären IAM-Lösungen.


### Einsatzmöglichkeiten

- Single Sign-On (SSO): Einmalige Anmeldung für mehrere Anwendungen und Dienste.
- Identity Federation: Integration mit externen Identitätsanbietern (z. B. LDAP, Active Directory, OAuth 2.0, OpenID Connect, SAML).
- Benutzerverwaltung: Rollen- und Rechteverwaltung für individuelle oder gruppenbasierte Zugriffskontrolle.
- Sicherheit: Unterstützung für Multi-Faktor-Authentifizierung (MFA), Passwort-Richtlinien und Token-basierte Authentifizierung.
- Erweiterbarkeit: Anpassbar durch eigene Themes, Erweiterungen und Custom-Skripte.
- Self-Service-Portal: Benutzer können ihre Passwörter zurücksetzen und persönliche Daten verwalten.

### Einsatz im Projekt

Keycloak ist der zentrale IDM und verwaltet die Berechtigungen und Zugriffe auf den MLA.


## Voraussetzungen

* Kubernetes 1.23+
* Helm 3.8.0+
* PV provisioner support in the underlying infrastructure

## Installation

```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update
helm install keycloak bitnami/keycloak -n fiware
```

## License

Copyright © 2024 ADDIX GmbH.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.