# Taxonomía operativa de emergencias tecnológicas y CBRN

Clasificar la consulta con una o más filas. Un evento puede cruzar tipos (ejemplo: sismo que dispara incendio en refinería).

El mapa jurídico nuclear es IAEA. El químico de armas es OPCW. El industrial transfronterizo es UNECE TEIA. El de amenaza natural es el otro pilar. No mezclar.

## Eventos tecnológicos (HIP 5 y 7 como primarios)

| Tipo | Qué es | Dónde buscar primero |
| --- | --- | --- |
| Químico industrial | Fuga, nube tóxica, explosión en planta o almacén | Regulador químico / ambiente / protección civil del país |
| Químico transporte | Mercancías peligrosas en carretera, ferrocarril, puerto o tubería | Autoridad de transporte + ficha ADR/RID/IMDG como mapa |
| Radiológico | Fuente huérfana, accidente médico o industrial con radiación (sin reactor) | Regulador nuclear/radiológico nacional |
| Nuclear | Reactor, ciclo de combustible, notificación IAEA, INES | Regulador nuclear + IAEA IEC |
| Biológico de laboratorio | Accidente de contención, toxina, agente como arma. No es un brote comunitario | Autoridad de bioseguridad + cruce a salud si hay casos |
| Presa | Rotura, sobrevertido, evacuación de valle | Autoridad de presas / recursos hídricos. No IAEA |
| Relaves | Rotura de presa de jales o estériles mineros | Autoridad minera + ambiente |
| Apagón / red | Colapso eléctrico, isla de red, hospitales a oscuras | Operador de red + regulador energético |
| Telecom / cable | Corte de cable submarino o backbone | Regulador de telecom + operador |
| Hidrocarburo / derrame | Petróleo o gas en mar, río o costa | Autoridad de derrames (NOSDRA, ITOPF como mapa, REMPEC si Mediterráneo) |
| Explosión industrial | Puerto, silo, nitrato, polvorín civil | Ambiente + protección civil + investigación forense del Estado |

## Figuras de respuesta (no son el evento)

| Figura | Qué es | No confundir con |
| --- | --- | --- |
| Regulador nuclear | Autoridad nacional de seguridad nuclear y radiológica | Operador de la planta |
| NAA OPCW | Autoridad Nacional de la Convención sobre las Armas Químicas | Ministerio de salud |
| IAEA IEC | Incident and Emergency Centre. Canal interestatal | NRC de EE.UU. |
| RANET | Red de asistencia IAEA. Se activa a pedido del Estado | Un equipo que se despliega solo |
| JEU | Joint Environment Unit UNEP/OCHA. Evaluación ambiental de emergencia | NDMO |
| Operador de red | Quien despacha electricidad o gas | El NDMO |

## Adyacentes (otro experto)

| Evento | Experto |
| --- | --- |
| Amenaza natural sin ángulo tecnológico | EXPERTO DESASTRES NATURALES |
| Brote, epidemia, PHEIC | EXPERTO SALUD PUBLICA |
| Conflicto, DIH, minas, UXO | Hermano conflicto (aún no abierto). Aquí solo el tramo IAEA/OPCW |
| Voluntarios, matching, salvaguardas | EXPERTO VOLUNTARIOS |
| Natech (natural dispara tech) | Este repo en el tramo tecnológico + [cruce-desastres.md](../../playbooks/cruce-desastres.md) |

## Cómo usarlo

1. Marca tipo de evento + figura de respuesta.
2. Abre la familia en [families/index.md](../families/index.md).
3. Abre el marco en [frameworks/index.md](../frameworks/index.md).
4. Si hay amenaza natural, abre [cruce-desastres.md](../../playbooks/cruce-desastres.md).
5. Si hay heridos o EMT, abre [cruce-salud.md](../../playbooks/cruce-salud.md).
