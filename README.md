# Proyecto_Aplicado_II

## Descripción de los Datos:

Existen 3 Dataset que se componen de la siguiente información:

+ DS_POLIZA_COBERTURA: (UTF-8, sep=";")
  + ID_POLIZA (string): id que identifica al seguro como unico
  + COBERTURA (string): Concepto particular del cual se resguarda el asegurado
  + COND_GENERAL (string:list): lista de Condicionados Generales Utilizados en la póliza. Este registro es único a nivel de ID_POLIZA
  + MONTO_ASEGURADO (float): Monto max en UF del cual se resguarda para una determinada cobertura
  + PRIMA_PACTADA (float): Monto en UF que se acuerda con el asegurado por dicha cobertura

Registro Unico: ID_POLIZA + COBERTURA

+ DS_POLIZA_VEHICULO: (UTF-8, sep=";")
    + ID_POLIZA (string): id que identifica al seguro como unico
    + FANOFA_T05 (int): Año de Fabricación del Vehiculo
    + MARCA (string): Marca del vehiculo. si existe más de una forma de escribirlo, estará separado por ";"
    + MODELO (string): Modelo del vehiculo

Registro Unico: ID_POLIZA

+ DS_SINIESTRO: (UTF-8, sep=";")
  + ID_SINIESTRO (string): id que identifica de manera única al Accidente/Siniestro
  + ID_POLIZA (string): id que identifica al seguro como unico
  + COBERTURA_AFECTADA (string): Concepto del seguro que se vio afectado por el Siniestro/Accidente
  + PROVISION_INICIAL (float): valor en UF, asociado al dinero que congelar la empresa aseguradora producto del accidente
  + GASTO_REAL (float): Gasto real en UF. a medida que el gasto se concreta, la provisión se libera.

Archivos Adicionales:

+ CondGeneral: (Carpeta)
  + Contiene archivos PDF asociado a las condiciones generales por la cual se rige el seguro ("contrato). está completamente ligado a la columna "COND_GENERAL" del archivo DS_POLIZA_COBERTURA.

+ CondParticular: (Carpeta)
  + Contiene en archivos tipo txt, todas las condiciones particulares (Empresa-Cliente) que se agregan a las condiciones generales. Cada ID_POLIZA, posee un archivo con sus propias particularidades.

+ RelatoDenuncio: (Carpeta)
  + Contiene en archivos tipo txt, todos los relatos de denuncios asociados a los Siniestros. cada ID_SINIESTRO debe poseer uno de estos.

