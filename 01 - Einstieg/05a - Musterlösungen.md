**Musterlösung zu Aufgabe 1 – Advanced Persistent Threats und E-Mail-Sicherheit in der Praxis**

1. **Analyse des Szenarios und genutzte Angriffsvektoren:**
    
    - APTs (Advanced Persistent Threats) zeichnen sich dadurch aus, dass Angreifer über einen langen Zeitraum sehr gezielt und unauffällig vorgehen. In diesem Fall deuten kleine, wiederkehrende Anomalien (ungewöhnliche Loginzeiten, sporadische, nicht nachvollziehbare Datenübertragungen) auf einen verdeckten Angreifer hin.
    - Mögliche Angriffsvektoren:
        - **Spear-Phishing:** Mitarbeiter könnten personalisierte schädliche Anhänge oder Links erhalten haben, die Schadsoftware ("Malware") installiert hat.
        - **Malware**: Zum Beispiel Trojaner, die Remote Access ermöglichen, oder Keylogger, die Zugangsdaten sammeln.
        - **Insider Threats**: Ein internes Konto könnte gekapert oder ein Mitarbeiter manipuliert worden sein.
        - **Exfiltration über scheinbar legitime Kanäle**: Datenabfluss versteckt durch legitime Tools und Kommunikationskanäle.
    - Die Angreifer nutzen gezielt Lücken in der täglichen Routine und bleiben durch "Low and Slow"-Taktiken (geringes Tempo, kleine Mengen) unterhalb der Radarschwelle der automatischen Überwachung.
2. **Herkömmliche Schutzmaßnahmen und ihre Grenzen bei APTs:**
    
    - **Black-/Whitelisting:**
        - Listen können umgangen werden, wenn z.B. Schadsoftware mit legitimen, whitelisted Anwendungen kommuniziert oder ihre Aktivitäten verschleiert.
        - Zero-Day-Angriffe (unbekannte Schwachstellen) und getarnte/angepasste Schadsoftware tauchen auf keiner Blacklist auf.
    - **E-Mail-Verschlüsselung:**
        - Verschlüsselung schützt zwar die Kommunikation, kann aber Angriffe nicht verhindern, die innerhalb der Organisation stattfinden, nachdem ein Gerät kompromittiert wurde.
        - Phishing-Angriffe funktionieren auch mit verschlüsselten E-Mails, falls die Benutzer in die Falle tappen.
    - **Antivirenprogramme & Firewalls:**
        - Können bekannte Bedrohungen erkennen, sind aber gegen neue Varianten und gezielte Angriffe oft machtlos.
        - Firewalls bieten keinen Schutz, wenn der Angreifer legitime Protokolle und Ports nutzt.
3. **Maßnahmenkatalog für Unternehmen:**
    - **Technische Maßnahmen:**
        - Etablierung eines "Defense in Depth"-Konzepts: Mehrere, aufeinander abgestimmte Schutzebenen.
        - _Network Segmentation_: Kritische Bereiche voneinander isolieren, um die seitliche Bewegung des Angreifers zu minimieren.
        - _Anomaly Detection_: Einsatz moderner Systeme zur Verhaltensanalyse (z.B. KI-gestützte Analyse ungewöhnlicher Aktivitäten).
        - _Threat Hunting_: Proaktives Suchen nach Anzeichen eines Angriffs, auch wenn keine Alarmierung vorliegt.
        - _Zero Trust-Modell_: Keine pauschalen Vertrauensstellungen – jede Anfrage wird erneut geprüft und authentifiziert.
        - _Monitoring_: Genaue Protokollierung und Auswertung von Login-Versuchen, Dateiübertragungen und Datenabflüssen.
        - _Einführung von Multi-Faktor-Authentifizierung (MFA)_ für kritische Systeme.
    - **Organisatorische Maßnahmen:**
        - Regelmäßige Security Awareness Trainings für Mitarbeitende (z.B. zum Erkennen von Spear-Phishing).
        - Definition klarer Meldewege für verdächtige Vorfälle und Verhaltensweisen.
        - Übung von Notfallplänen, um im Ernstfall schnell reagieren zu können.
        - Zusammenarbeit mit externen IT-Security-Experten, um Schwachstellen regelmäßig zu überprüfen (Penetration Testing, Schwachstellenscans).

---

**Musterlösung zu Aufgabe 2 – Botnetze, DDoS und Passwortrichtlinien im Unternehmensalltag**

4. **Analyse der Angriffsweise und paralleler Zugriffsversuche:**  
   - **DDoS durch Botnetze:**  
     - Angreifer infizieren eine Vielzahl fremder Computer (durch Malware) und steuern diese zentral.  
     - Diese „Bots“ senden gleichzeitig massenhaft Anfragen an den Web-Server des Unternehmens.  
     - Ziel ist es, den Server zu überlasten, ihn unbenutzbar zu machen oder als Ablenkung für weitere Angriffe zu nutzen.
   - **Interne Zugriffsversuche:**  
     - Die Vielzahl fehlerhafter Login-Versuche im Firmennetzwerk deutet auf einen Brute-Force-Angriff oder Credential Stuffing hin.  
     - Angreifer könnten versuchen, schwache oder gestohlene Zugangsdaten zu benutzen, um sich Zugang zu Konten mit administrativen Rechten zu verschaffen.  
     - Die zeitliche Nähe beider Vorfälle spricht für eine koordinierte Attacke, bei der der DDoS-Angriff als Ablenkung dient, während parallel Versuche laufen, Konten im Unternehmensnetz zu übernehmen.

2. **Rolle schwacher Passwörter, Blacklisting und Whitelisting:**  
   - **Schwache Passwörter:**  
     - Einfache oder mehrfach verwendete Passwörter lassen sich durch automatisierte Angriffe leicht herausfinden.  
     - Passwörter, die auf Blacklists stehen (beispielsweise bekannte Begriffe oder in früheren Leaks aufgetauchte Kombinationen), bieten kaum Schutz.
   - **Blacklisting:**  
     - Bei der Authentifizierung können bekannte schwache oder kompromittierte Passwörter blockiert werden.  
     - Ebenfalls möglich ist das Blacklisting bekannter Angriffs-IP-Adressen.
   - **Whitelisting:**  
     - Beschränkung des Zugangs auf bestimmte IP-Bereiche oder Geräte (z.B. VPN), sodass nur autorisierte Personen/Systeme Zugriff erhalten.  
     - Reduziert die Angriffsfläche, da nicht jeder Nutzer oder jede IP versuchen kann, sich einzuloggen.

3. **Umfassendes Schutzkonzept:**  
   - **Technische Maßnahmen:**  
     - Einführung und technische Durchsetzung starker Passwortrichtlinien (Mindestlänge, Komplexität, keine Wiederverwendung).  
     - Einsatz von Account-Locking (Konto-Sperre nach mehreren Fehlversuchen; gegebenenfalls gestaffelt nach Account-Typ).  
     - Multi-Faktor-Authentifizierung (MFA) für besonders kritische Konten und Dienste.  
     - Monitoring und Echtzeit-Alarmierung bei ungewöhnlichem Login-Verhalten oder DDoS-Mustern.  
     - Einsatz von dedizierten DDoS-Schutzlösungen (z.B. Rate Limiting, vorgelagerte Filter über Dienstleister, Captcha-Schutz).  
     - Netzwerksegmentierung: Kritische Systeme werden vom öffentlichen Netz sowie vom restlichen Firmen-LAN getrennt.  
     - Regelmäßige Prüfung von Zugriffsrechten und Benutzerkonten auf Aktualität.
   - **Organisatorische Maßnahmen:**  
     - Mitarbeitende regelmäßig zu sicherem Passwortumgang und Social Engineering schulen.  
    