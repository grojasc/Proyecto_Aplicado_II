# Proyecto_Aplicado_II

## Descripción de los Datos:

la base de datos es un archivo pickle, de un dataframe

### **Sus columnas son las siguientes:**
<hr>

versión 2 (datos_v2.pkl)

**ID_SINIESTRO**: (string) identificador único del siniestro reportado.

**ID_POLIZA**: (string) identeificador único de la póliza.

**RELATO**: (string) texto anonimizado, del relato del siniestro.

**MODELO**: (string) Modelo del vehiculo registrado.

**MARCA**: (string) Marca del vehiculo registrado.

**ANIO**: (string) Año de Fabricación del modelo.

**COBERTURA_POLIZA**: ( list(string) ) lista de string asociado a las coberturas homologadas de la póliza.

**COBERTURA_SINIESTRO**: ( list(string) ) lista de string asociado a las coberturas homologadas afectadas en el siniestro.

**PROVISION_INICIAL**: ( list(float) ) lista de valores en UF de la provision inicial asociada a la COBERTURA_SINIESTRO.

**GASTO_UF**: ( list(float) ) Gasto real en UF asociada a la COBERTURA_SINIESTRO.

**FIN**: ( string ) columna separadora de cambios solo contiene tres astericos.

**COBERTURA_POLIZA_v2**: ( tupla(int)) tupla que repesenta la existencia de la coberturas Responsabilidad Civil (RC), Daños Materiales Parciales (DM) y Otras coberturas (OT) representadas (RC, DM, OT)

**COBERTURA_SINIESTRO_v2**: ( tupla(int)) tupla que repesenta la presencia de la coebertura afectada Responsabilidad Civil (RC), Daños Materiales Parciales (DM) y Otras coberturas (OT) representadas (RC, DM, OT)

**PROVISION_INICIAL_v2**: ( tupla(float)) tupla que acumula el valor en uf de la provision inicial (RC, DM OT)

**GASTO_REAL_v2**: ( tupla(float)) tupla que acumula el valor en uf del Gasto Real (RC, DM OT)