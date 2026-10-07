# Nunner

**La fede non va in pensione · Faith never retires**

Suor Gertrude, 70 anni, zero pazienza, contro i sette peccati capitali.
Un endless runner in pixel art che si gioca gratis nel browser, su PC e smartphone.

▶ **[www.playnunner.com](https://www.playnunner.com)**

[Italiano](#italiano) · [English](#english)

---

## Italiano

### La storia

Estate 1974: Gertrude, vent'anni, vince la finale dei 1500 metri. Poi appende la medaglia al chiodo e si fa suora.
Cinquant'anni dopo Settevizi, la città del peccato, chiede preghiere. Nessuno ci va da anni. Gertrude ci va, con le scarpe del '74.

L'intro, di circa mezzo minuto, parte da sola la prima volta. Si salta con un tasto o un tocco e si può rivedere dalla schermata iniziale.

### Come si gioca

Gertrude corre da sola. Tu la fai saltare.

| Azione | Tastiera e mouse | Telefono |
|---|---|---|
| Salto | `Spazio`, `↑`, `W` o clic | tocco |
| Salto più alto | tieni premuto | tieni premuto |
| Doppio salto | di nuovo, in aria | di nuovo, in aria |
| Pausa | `P` o `Esc` | pulsante in alto a destra |
| Musica | `M` | pulsante in alto a destra |

### I sette peccati: da saltare

Toccarne uno costa una vita e riporta Gertrude all'ultima croce. Le vite sono tre.

| Peccato | Aspetto | Dove sta |
|---|---|---|
| Superbia | lo specchio | a terra o in aria, fermo |
| Avarizia | il sacco d'oro | a terra, fermo |
| Lussuria | il tacco a spillo | a terra, fermo |
| Invidia | l'occhio verde | in aria, ondeggia |
| Gola | la torta | a terra, fermo |
| Ira | la bomba | a terra, saltella |
| Accidia | il cuscino | in aria, galleggia pigro |

I peccati arrivano a ondate e girano alla pari: esce sempre quello visto meno volte.

### Le sette grazie: da prendere

| Grazia | Oggetto | Effetto |
|---|---|---|
| Scudo della Fede | rosario | 7 s immune: i peccati che tocchi si frantumano |
| Ali dello Spirito | colomba | 6 s di volo: gravità leggera, salti infiniti |
| Pazienza | clessidra | 6 s col mondo a metà velocità |
| Purificazione | acqua santa | cancella tutti i peccati sullo schermo |
| Carità | Sacro Cuore | una vita in più (massimo 3) |
| Gloria | stella | 10 s di punti doppi, e le grazie vengono a te |
| Umiltà | giglio | 8 s piccola, per passare sotto i peccati |

### Punti, croci e livelli

- **5 punti** a ogni metro di strada.
- **+50** a ogni grazia, **+25** per ogni peccato frantumato con lo Scudo, **+30** per ogni peccato cancellato dall'Acqua santa, **+100** per il Sacro Cuore preso con le vite già piene. La Gloria raddoppia tutto.
- **Una croce ogni 180 m**: vale +200 e salva il punto da cui si riparte.
- **Ogni 300 m** si sale di livello: la corsa accelera, fino a 2,5 volte la velocità iniziale, e arrivano ondate più difficili.
- Quando batti il record partono i fuochi d'artificio. A fine partita c'è la tua *via crucis*: quali peccati ti hanno tolto le vite, con un versetto della Bibbia per quello che ti ha battuto.

### Il mondo

Settevizi ha un ciclo giorno e notte (alba, giorno, vespro, notte) che scorre col tempo e non con i metri. Ci sono pioggia e lampi, il traffico, la volante che insegue il ladro, i piccioni, il sassofonista all'angolo, la metropolitana sulla sopraelevata e un palazzo per ogni peccato. La colonna sonora è un noir jazz a 8 bit che accelera con la corsa.

### Struttura del progetto

```
index.html                  il gioco intero: HTML, CSS e JavaScript in un solo file
nunner_anteprima_it.png     l'immagine che compare quando si condivide il link
LICENSE                     tutti i diritti riservati
```

Il gioco non usa librerie né file esterni e non serve compilarlo: si apre `index.html` nel browser. Tutta la grafica è disegnata dal codice, partendo da mappe di caratteri, a bassa risoluzione e ingrandita a pixel interi. Musica ed effetti sono sintetizzati in tempo reale con la Web Audio API. Dall'esterno arrivano solo i font, da Google Fonts.

Il codice di `index.html` è diviso in sezioni numerate:

| Sezione | Contenuto |
|---|---|
| 1–3 | base del canvas, font bitmap 3x5 e 5x7, sprite da mappe di caratteri |
| 4–7 | Suor Gertrude, i peccati, le lingue, le grazie, costruzione degli sprite |
| 8–9 | ciclo giorno e notte, scenografia della città |
| 10–16 | stato di gioco, particelle, generazione delle ondate, grazie, croci, salto, aggiornamento |
| 17–19 | disegno del mondo, HUD, fotogramma |
| 20 | effetti sonori e musica |
| 21 | schermate, lingue, contatore delle visite, intro animata con la sua colonna sonora |
| 22–24 | dimensioni dello schermo, input, ciclo principale e avvio |

### Dati salvati e privacy

Il gioco salva nel browser (`localStorage`) solo il record, la lingua, la musica accesa o spenta e se l'intro è già stata vista. Non usa cookie. Le visite sono contate con [GoatCounter](https://www.goatcounter.com), che non usa cookie né traccia le persone; il totale compare nella schermata iniziale come numero di "fedeli".

### Licenza

© 2026 Carolina Crespi. Tutti i diritti riservati: puoi giocare e leggere il codice, ma non copiarlo né riusarlo senza permesso. Dettagli in [LICENSE](LICENSE).

---

## English

### The story

Summer 1974: Gertrude, aged twenty, wins the 1500 metres final. Then she hangs up her medal and becomes a nun.
Fifty years later Settevizi, the city of sin, begs for prayers. No one has gone there in years. Gertrude goes, in her shoes from '74.

The intro, about half a minute long, plays by itself the first time. Any key or tap skips it, and it can be replayed from the title screen.

### How to play

Gertrude runs on her own. You make her jump.

| Action | Keyboard and mouse | Phone |
|---|---|---|
| Jump | `Space`, `↑`, `W` or click | tap |
| Higher jump | hold | hold |
| Double jump | again, in mid-air | again, in mid-air |
| Pause | `P` or `Esc` | button top right |
| Music | `M` | button top right |

### The seven sins: jump over them

Touching one costs a life and sends Gertrude back to the last cross. She has three lives.

| Sin | Looks like | Where |
|---|---|---|
| Pride | the mirror | on the ground or in the air, still |
| Greed | the bag of gold | on the ground, still |
| Lust | the stiletto heel | on the ground, still |
| Envy | the green eye | in the air, bobbing |
| Gluttony | the cake | on the ground, still |
| Wrath | the bomb | on the ground, hopping |
| Sloth | the pillow | in the air, drifting lazily |

Sins come in waves and take turns fairly: the one seen least so far always comes next.

### The seven graces: grab them

| Grace | Object | Effect |
|---|---|---|
| Shield of Faith | rosary | immune for 7 s: sins you touch shatter |
| Wings of the Spirit | dove | fly for 6 s: light gravity, endless jumps |
| Patience | hourglass | the world runs at half speed for 6 s |
| Purification | holy water | wipes out every sin on screen |
| Charity | Sacred Heart | one extra life (max 3) |
| Glory | star | double points for 10 s, and graces come to you |
| Humility | lily | shrink for 8 s and slip under the sins |

### Points, crosses and levels

- **5 points** per metre.
- **+50** per grace, **+25** per sin shattered by the Shield, **+30** per sin wiped out by Holy water, **+100** for a Sacred Heart caught with full lives. Glory doubles everything.
- **A cross every 180 m**: worth +200, and it saves the point you restart from.
- **Every 300 m** you level up: the run speeds up, to 2.5 times the starting speed, and harder waves appear.
- Beat your best and the fireworks go off. At the end of a run you see your *way of the cross*: which sins took your lives, with a Bible verse for the one that got you.

### The world

Settevizi has a day and night cycle (dawn, day, evening, night) that follows time, not distance. There is rain and lightning, traffic, a police car chasing a thief, pigeons, a sax player on the corner, a train on the elevated line and one building for each sin. The soundtrack is 8-bit noir jazz that speeds up with the run.

### Project structure

```
index.html                  the whole game: HTML, CSS and JavaScript in one file
nunner_anteprima_it.png     the image shown when the link is shared
LICENSE                     all rights reserved
```

The game uses no libraries and no external files, and there is no build step: just open `index.html` in a browser. All the artwork is drawn by the code from character maps, at low resolution and scaled up by whole pixels. Music and sound effects are synthesised live with the Web Audio API. Only the fonts come from outside, from Google Fonts.

The code in `index.html` is split into numbered sections:

| Section | Contents |
|---|---|
| 1–3 | canvas basics, 3x5 and 5x7 bitmap fonts, sprites from character maps |
| 4–7 | Sister Gertrude, the sins, languages, the graces, sprite building |
| 8–9 | day and night cycle, city scenery |
| 10–16 | game state, particles, wave generation, graces, crosses, jumping, update |
| 17–19 | drawing the world, HUD, frame |
| 20 | sound effects and music |
| 21 | screens, languages, visit counter, animated intro with its soundtrack |
| 22–24 | screen size, input, main loop and start-up |

The comments in the code are in Italian.

### Saved data and privacy

The game stores only the best score, the language, the music setting and whether the intro has been seen, in the browser (`localStorage`). It uses no cookies. Visits are counted with [GoatCounter](https://www.goatcounter.com), which uses no cookies and does not track people; the total is shown on the title screen as the number of "faithful".

### Licence

© 2026 Carolina Crespi. All rights reserved: you can play and read the code, but not copy or reuse it without permission. Details in [LICENSE](LICENSE).
