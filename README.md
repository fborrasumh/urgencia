# UrgencIA

Urgencias en la consulta de medicina estética. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/urgencia/

**Idiomas:** español (por defecto), inglés, portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

Primera app del [Kit EstéticIA](https://fborrasumh.github.io/kitesteticia/): los protocolos de urgencia de la consulta de medicina estética en pantalla.

- **Cinco urgencias**: oclusión vascular, pérdida de visión o síntomas neurológicos tras un relleno, anafilaxia, toxicidad sistémica por anestésico local y síncope vasovagal. Los botones están lo primero en la portada.
- **Ayuda para elegir**: seis preguntas de sí o no y reglas fijas, en orden de prioridad, que proponen el protocolo.
- **Reloj y registro**: al empezar corre el reloj; cada paso marcado y cada fármaco administrado quedan anotados con su hora, igual que las constantes y las notas. Se puede deshacer el último registro y cambiar de protocolo sin perder lo hecho.
- **Dosis calculadas** con el peso del paciente y los valores de la consulta: hialuronidasa por zona isquémica y su volumen según el vial, adrenalina intramuscular y emulsión lipídica al 20 % (bolo, perfusión y máximo acumulado). Los intervalos de repetición se cuentan en pantalla, con aviso sonoro opcional.
- **Informe de traslado** escrito a partir del registro: datos, procedimiento (producto, lote, zona, volumen), cronología, fármacos, constantes, situación final y protocolo de referencia. Word, impresión o PDF y copia en texto. Los informes quedan archivados.
- **Carro de urgencias**: caducidad de cada elemento, aviso de lo caducado y de lo que caduca en 30 días, y registro de la revisión mensual.
- **Protocolos de la consulta**: cada valor de dosis lleva su fuente y se puede ajustar al protocolo escrito y a los productos de la consulta.
- **Modo simulacro** para practicar con el equipo: todo queda marcado como simulacro, también en el informe.

No usa IA y no hace ninguna llamada de red: funciona sin conexión una vez abierta. Español, inglés y portugués.

## Fuentes de los protocolos

- DeLorenzi C. New high dose pulsed hyaluronidase protocol for hyaluronic acid filler vascular adverse events. Aesthet Surg J 2017;37(7):814-825. doi:10.1093/asj/sjw251
- Beleznay K et al. Update on avoiding and treating blindness from fillers: a recent review of the world literature. Aesthet Surg J 2019;39(6):662-674. doi:10.1093/asj/sjz053
- Resuscitation Council UK. Emergency treatment of anaphylaxis: guidelines for healthcare providers. 2021.
- Neal JM, Neal EJ, Weinberg GL. ASRA Local Anesthetic Systemic Toxicity checklist: 2020 version. Reg Anesth Pain Med 2021;46(1):81-82. doi:10.1136/rapm-2020-101986
- Brignole M et al. 2018 ESC Guidelines for the diagnosis and management of syncope. Eur Heart J 2018;39(21):1883-1948. doi:10.1093/eurheartj/ehy037

## Privacidad

Todo se guarda en el navegador: urgencias, registro, informes, carro y valores del protocolo. Nada sale hacia ningún servidor. Se recomienda usar un identificador en lugar del nombre del paciente.

## Límites

Es una ayuda para médicos formados en el manejo de estas urgencias. No es un producto sanitario y no sustituye al protocolo escrito de la consulta, a las fichas técnicas, a la formación en soporte vital ni al juicio clínico. Los valores de dosis son los de las fuentes citadas y cada consulta debe comprobarlos y ajustarlos a su protocolo y a sus productos. Las técnicas intraorbitarias o retrobulbares no se incluyen: corresponden al centro receptor. Ante la duda, llamar al teléfono de emergencias.

## Pruebas

`node tests/test_nucleo.js` (dosis, triaje, carro e informe) y `python3 tests/smoke.py` (recorrido completo en Chromium, tres idiomas, persistencia, accesibilidad WCAG 2.2 AA, CSP y móvil).

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche) y Elena Caride Miana (Dra. Caride Medicina Estética & Antiaging).

Primera app del Kit EstéticIA, diseñado para el alumnado del Máster de Formación Permanente en Medicina Estética Integral y Antienvejecimiento (UMH).

ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573) · Elena Caride Miana [0000-0002-7620-4857](https://orcid.org/0000-0002-7620-4857)

## Cómo citar

Borrás Rocher, F. y Caride Miana, E. (2026). *UrgencIA* (v1.0.0) [Software]. (DOI en trámite)

## Licencia

MIT. Véase [LICENSE](LICENSE).
