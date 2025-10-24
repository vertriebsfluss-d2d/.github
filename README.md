# Vertriebsfluss – Interne Door-to-Door Karten-App
### Überblick

Eine interne mobile App zur Unterstützung des Door-to-Door-Vertriebs. Mitarbeitende sehen eine Karte, markieren besuchte Häuser und synchronisieren ihre Positionen in Echtzeit mit dem Team. Ziel ist transparente Gebietsabdeckung, Vermeidung von Doppelbesuchen und effizientere Tourenplanung.

### Kernfunktionen
- Karte mit Marker für Häuser, Besuchsstatus und Notizen.
- Live-Standortfreigabe der Mitarbeitenden innerhalb ihres Teams.
- Echtzeit-Synchronisation von neuen/aktualisierten Markern.
- Cluster-Darstellung für hohe Markerdichte.
- Rollen- und Teambasierte Zugriffskontrolle.

### Architekturüberblick
- Flutter (iOS/Android) MVVM, Provider/Consumer
- Karten: Google Maps
- Firestore für Dokument und Metadaten (Häuser, Teams, Stammdaten)
- PostgreSQL + PostGIS für komplexere Geodatenabfrage
- Echtzeit Web-Socket-Server (backend) und Client (frontend) für Mitarbeiter Standorte und Echtzeit Synchronisation neuer Marker
