# Esquema de ficha país

Cada país o territorio usa este bloque. Campos vacíos se escriben `por verificar en vivo`, nunca se inventan.

```
## [ISO2] [Nombre en español]
- iso3: XXX | idiomas: códigos BCP-47
- nombre_local: nombre del Estado en idioma oficial
- nuclear_regulator: autoridad de seguridad nuclear y radiológica
- nuclear_url: URL del regulador (si está comprobada)
- chemical_authority: autoridad de accidentes químicos / industriales
- environment: ministerio o agencia ambiental
- dam_or_mining: presas, relaves o minería
- energy_or_infra: red eléctrica, hidrocarburos, telecom
- opcw_naa: Autoridad Nacional CWC (si está publicada)
- iaea_notes: miembro, planta, o "sin programa de potencia"
- regional: FORO / ASEANTOM / ENSREG / AFRA / REMPEC / otro
- notas
```

Fuentes semilla: directorio IAEA de reguladores, lista de Autoridades Nacionales OPCW, puntos focales TEIA, directorio ICOLD. Verificar URL en vivo.

IAEA: https://www.iaea.org/
OPCW NAA: https://www.opcw.org/
UNECE TEIA: https://unece.org/environment-policy/industrial-accidents
