
### Hashes de contraseñas
| Hash | Formato |
|------|---------|
| `$argon2id$v=19$m=65536,t=4,p=1$TmRXZG56SW5aNGJTckhDYw$ehzw1inl8w3qN/pFhG9wkXLzYNyjQzn67Ketu9gjIIA:C7fPstzt` | Argon2 |
| `0x2432792431302463556f4c58615144486d35786b754b7044677350562e4c774c4978562f743678666c6156744b7a575964514d6135784c5956673269` | Binary (hex) |

---

## 📎 Actividad en VirusTotal (KiraSecurity)

| Colección / Graph | Fecha |
|------------------|-------|
| shinyhunte.red +NUDOS | 2026-06-09 |
| Lizard Squad - Killnet - proxis killnet - Malwares, BOTNET, WORMS, PHISHING | 2026-05-31 |
| www.shinyhunte.red 185.199.111.153 | 2026-05-28 |

---

## 🎯 Conclusiones

1. **shinyhunte.red era infraestructura oficial de ShinyHunters** - Confirmado por múltiples fuentes y por observación directa.
2. **El dominio estuvo activo** - Operaba como sitio de "prueba de vida" y extorsión durante el periodo de investigación.
3. **Actualmente está caído** - Verificado mediante check-host y múltiples fuentes.
4. **Compartía infraestructura con otras amenazas** - Nodos de Killnet, CyberVolk y Lizard Squad presentes.
5. **Patrón consistente** - El uso de dominios clearnet (.rs, .red) es un TTP documentado del grupo.
6. **Alta rotación de activos** - Los certificados SSL cambiaron rápidamente y el dominio resolvía a IPs de Cloudflare/Fastly para evadir bloqueos.

---

## 📝 Recomendaciones

| Acción | Prioridad |
|--------|-----------|
| **Bloquear** shinyhunte.red y las IPs asociadas (185.199.111.153, 172.67.214.117, 104.21.93.206) | 🔴 ALTA |
| **Monitorear** nuevos dominios que sigan el patrón shinyhunte.* (rs, red, etc.) | 🟠 MEDIA |
| **Alertar** sobre correos entrantes desde dominios protonmail.ch o tutanota.com en contexto de extorsión | 🟠 MEDIA |
| **Compartir IOCs** con plataformas de Threat Intelligence (MISP, OpenCTI) | 🟡 BAJA |
| **Investigar** otros dominios en el rango 185.199.108.0/22 | 🟡 BAJA |

---

## 📚 Fuentes

- [VirusTotal - shinyhunte.red](https://www.virustotal.com/gui/domain/shinyhunte.red)
- [VirusTotal - IP 185.199.111.153](https://www.virustotal.com/gui/ip-address/185.199.111.153)
- [X - Dominic Alvieri (@AlvieriD)](https://x.com/AlvieriD)
- [X - @none_028](https://x.com/none_028)
- [WatchGuard - ShinyHunters Infrastructure](https://www.watchguard.com/wgrd-news/cyber-security-updates/uncategorized-cyber-security-updates/shinyhunters-infrastructure)
- [Zensec - ShinyHunters Analysis](https://www.zensec.co.uk/post/shinyhunters)
- [Seqrite - SLSH Coalition Report](https://www.seqrite.com/blog/slsh-coalition-shinyhunters-scattered-spider-lapsus/)
- [Constella Intelligence - ShinyHunters Tactics](https://constella.com/resources/webinars-events/)

---

## 📎 Anexo: Perfil OSINT del Operador (KromSec / Spid3r / AnonymousTurkey)

El análisis de infraestructura se complementó con una investigación OSINT sobre el presunto operador del grupo, revelando un perfil público extenso y consistente con las tácticas de la amenaza.

### Identidad y alcance

| Campo | Valor |
|-------|-------|
| **Alias principales** | KromSec, Spid3r, AnonymousTurkey, YourAnonSpider, whiteblue_bl00d, 0wlhexus |
| **ID de Telegram** | 5119060622 |
| **Registro** | Enero - Abril 2022 |
| **Grupos en Telegram** | Breached Data (@BreachedDB), DogelonMars (@DogelonMars), Pentester Chat (@PentesterChat) |
| **Canal principal** | @Krom_Sec, @spid3rcrypto, @YourAnonSpider, @anoncollectivechat, @siegedsec |
| **Perfil estimado** | 30-40 años, manejo de al menos 7 idiomas. Motivación principal: beneficio económico (venta de datos, botnets). Utiliza fachada de hacktivismo político. |
| **Red de contactos** | Conexiones confirmadas con grupos pro-rusos (Killnet) y actores en Oriente Medio. |

### Mensaje público en persa (Telegram @Krom_Sec)

> *"درود به مردم ایران، امروز به شما اعلام می کنیم که سازمان فناوری اطلاعات ایران [ito.gov.ir] هک شده است. با اینکه سیستم فقط کامپیوترهای متصل به شبکه خصوصی "فوق العاده امن" را می پذیرفت، پسورد و اطلاعات را به دست آوردیم. ... ما به آزادی اعتقاد داریم و برای اعتقادات خود به مبارزه ادامه میدهیم."*
>
> *"We are KromSec. Expect Us! We share the information of government employees, use it well."*

### Correos electrónicos y contraseñas filtradas

| Correo electrónico | Contraseña / Hash | Contexto |
|--------------------|-------------------|----------|
| `i.spider.bernard@gmail.com` | `Spid3rBlackBernard420` | Filtración LinkPass (2022) y Cloudata (2023) |
| `i.spid3r.bernard@gmail.com` | `Spid3rBlackBernard420` | Variante del mismo operador |
| `0wlhexus@gmail.com` | `prussiaisawesome` | Filtración Wattpad (2020) |
| `0wlhexus@gmail.com` | `518422e5c1f6a47e828a460b297f297d5dcf261f0a4fa59b36c57290c6f29394` | Hash bcrypt (Wattpad) |
| `YourAnonSpider@protonmail.com` | Hash Argon2 | Perfil AnonymousTurkey |
| `YourAnonSpider@riseup.net` | Hash Argon2 | Perfil AnonymousTurkey |
| `el_cobra69@hotmail.com` | - | Asociado a @siegedsec |
| `shinyc0rp@tuta.io` | - | Correo histórico del grupo |

### Fugaz de datos asociadas

| Filtración | Año | Descripción |
|------------|-----|-------------|
| **LinkPass collection** | 2022 | ~150M credenciales robadas de navegadores. Contiene apodos, correos, teléfonos y contraseñas en texto plano. |
| **Cloudata** | 2023 | Recopilación de 338 GB (~11B líneas) de correos y contraseñas. Post-deduplicación: ~2B líneas. |
| **Wattpad** | 2020 | ~270M registros: nombres, correos, IPs, género, fecha de nacimiento y contraseñas hasheadas con bcrypt. |
| **Domains-Monitor.com** | 2025 | Descarga de 275M registros de URLs (solo direcciones, sin otros datos). |

### Actividad y campañas

| Actividad | Año | Descripción |
|-----------|-----|-------------|
| **#OpIran** | 2022-2024 | Ataques contra gobierno iraní (ito.gov.ir, Ministerio de Industrias y Minas, Organización Nacional de Normalización) |
| **DDoS Chechenia** | 2024 | Ataques contra objetivos en Rusia |
| **SiegedSec** | 2023-2026 | Operación de dominios siegedsec.com, .locker, .ru |

### Dominios asociados al operador

| Dominio | Estado |
|---------|--------|
| siegedsec.com | Activo (histórico) |
| siegedsec.locker | Dominio de extorsión |
| siegedsec.ru | Variante rusa |
| shinyhunte.rs | Suspendido (mayo 2026) |
| shinyhunte.red | Caído (post-junio 2026) |

### Huella en redes sociales y plataformas (YourAnonSpider)

| Categoría | Plataformas |
|-----------|--------------|
| **Social** | Facebook, Twitter/X, Instagram, Ello, Bluesky, Threads, Weibo, Xiaohongshu, Gettr, Truth Social |
| **Mensajería** | Telegram, Discord |
| **Tech** | HackerNews, Indie Hackers |
| **Arte** | Newgrounds |
| **Dev** | GitHub, Glitch |
| **Programación** | HackerRank, CodeChef, CodinGame |
| **Gaming** | Steam, Nintendo, Armor Games, Game Jolt |
| **Streaming** | Twitch, Trovo, DLive |
| **Música** | YouTube Music |
| **Video** | YouTube, Bitchute, DTube, LBRY, Odysee |
| **Dating** | Plenty of Fish, Scruff |
| **Freelance** | Freelancer |
| **Blog** | WordPress |
| **NFT** | Nifty Gateway |
| **Crypto** | Etherscan |
| **Seguridad** | TryHackMe, Root-Me |
| **Educación** | Duolingo |
| **Deporte** | MapMyRun, Garmin Connect |

> **Nota:** Muchos de estos perfiles pueden estar inactivos o ser señuelos, pero la consistencia del alias y su asociación con correos electrónicos y fugas validadas aumenta significativamente su credibilidad como huella del actor de amenaza.

---

## 📎 Anexo: Línea de tiempo de la investigación

| Fecha | Evento |
|-------|--------|
| 2020-06 | Filtración Wattpad (~270M registros) |
| 2022 | Filtración LinkPass (~150M credenciales) |
| 2022-04 | Registro del ID de Telegram 5119060622 |
| 2023-05-18 | Recopilación de datos Cloudata (338 GB) |
| 2025-07-06 | Descarga de Domains-Monitor.com (275M URLs) |
| 2026-01 | WatchGuard documenta shinyhunte.rs |
| 2026-05-02 | Creación del dominio shinyhunte.red |
| 2026-05-26 | Primer avistamiento público por Dominic Alvieri |
| 2026-05-28 | Creación de colecciones en VT (www.shinyhunte.red) |
| 2026-05-31 | Documentación de correlación con Killnet/CyberVolk/Lizard Squad |
| 2026-06-09 | Creación de graph "shinyhunte.red +NUDOS" y finalización del análisis |
| Post-2026-06-09 | Verificación de caída del dominio mediante check-host |

---

*Este informe forma parte del portafolio CTI de Condor2026.*  
*Investigación asistida por software propio **Andrómeda Universo 25**.*

*Caso cerrado: ✅ CONFIRMADO - Infraestructura maliciosa de ShinyHunters (actualmente caída)*
