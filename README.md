Reflow-Ofen Einweisung
======================

Einweisung des [FAU FabLab](https://fablab.fau.de) in den [Reflow-Ofen](https://fablab.fau.de/tool/reflow-ofen) mit Reflow-Controller.

Inhalt
------

- Gefahren und Verhaltensregeln (Betriebsanweisung)
- Lötpaste: Umgang, Aufbringen mit Stencil oder Dispenser
- Vorbereitung des Ofens, Durchführung des Reflow-Prozesses, Abbau
- Kosten

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/reflow-ofen-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/reflow-ofen-einweisung/einweisung_reflow-ofen.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/reflow-ofen-einweisung/Einweisungsliste_Reflowofen.pdf)
- [Betriebsanweisung](https://brain.fablab.fau.de/build/reflow-ofen-einweisung/betriebsanweisung_reflow-ofen.pdf) (Aushang)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/reflow-ofen-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/reflow-ofen-einweisung.git
cd reflow-ofen-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/reflow-ofen-einweisung/status.svg)](https://brain.fablab.fau.de/build/reflow-ofen-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/reflow-ofen-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/reflow-ofen-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/reflow-ofen-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/reflow-ofen-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
