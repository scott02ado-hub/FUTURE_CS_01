🟡 FINDING 1 — Weak CORS Configuration
📌 Evidence
Access-Control-Allow-Origin: *
Access-Control-Allow-Origin: http://localhost:4200
⚠️ Risk Level

🟡 Medium

🧠 Explication simple

Le serveur autorise des origines externes à accéder aux ressources.

💼 Impact business
Possible accès non contrôlé aux données côté client
Risque d’exploitation via sites malveillants
Mauvaise configuration API
🔧 Remediation
Restrict CORS policy to trusted and production domains only.
Avoid using wildcard (*) in production environments.
🟡 FINDING 2 — Multiple Technology Exposure (Heroku + Apache)
📌 Evidence
Server: Heroku
Server: Apache/2.4.67 (Unix)
⚠️ Risk Level

🟡 Medium

🧠 Explication

Le système expose plusieurs couches d’infrastructure :

cloud (Heroku)
serveur web (Apache)
💼 Impact business
facilite la reconnaissance de l’architecture
aide les attaquants à cibler des vulnérabilités connues
🔧 Remediation
Minimize technology stack disclosure in HTTP headers.
Use security hardening and reverse proxy configuration.
🟡 FINDING 3 — API / Socket.IO Exposure
📌 Evidence
/socket.io/?EIO=4&transport=polling
⚠️ Risk Level

🟡 Medium

🧠 Explication

Communication en temps réel exposée via WebSocket / polling.

💼 Impact business
surface API exposée
peut être ciblée par abus ou flood logique
nécessite contrôle d’accès
🔧 Remediation
Implement authentication and rate limiting on real-time communication endpoints.
🟢 FINDING 4 — Security Headers Present (Positive)
📌 Evidence
X-Content-Type-Options: nosniff
X-Frame-Options: SAMEORIGIN
✅ Risk Level

Low (Good security practice)

💼 Impact

Protège contre :

clickjacking
MIME sniffing
👍 Conclusion

Bonne base de sécurité navigateur.

🟡 FINDING 5 — HTTP 403 Apache Endpoint
📌 Evidence
HTTP/1.1 403 Forbidden
Server: Apache/2.4.67
⚠️ Risk Level

Low / Informational

🧠 Explication

Un endpoint restreint existe mais révèle des informations serveur.

💼 Impact business
reconnaissance de services internes
aide à la cartographie du système
