# Comparing `tmp/omie-0.1.1.tar.gz` & `tmp/omie-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omie-0.1.1.tar", last modified: Tue May  7 14:14:51 2024, max compression
+gzip compressed data, was "dist/omie-0.2.1.tar", last modified: Tue May 21 13:31:38 2024, max compression
```

## Comparing `omie-0.1.1.tar` & `omie-0.2.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 14:14:51.986116 omie-0.1.1/
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       24 2024-05-07 14:04:48.000000 omie-0.1.1/MANIFEST.in
--rw-r--r--   0 aorellana  (1000) aorellana  (1000)      268 2024-05-07 14:14:51.986116 omie-0.1.1/PKG-INFO
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      230 2024-05-07 12:42:42.000000 omie-0.1.1/README.md
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 14:14:51.970116 omie-0.1.1/omie/
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       55 2024-05-07 12:42:42.000000 omie-0.1.1/omie/__init__.py
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5904 2024-05-07 12:42:57.000000 omie-0.1.1/omie/omie.py
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 14:14:51.970116 omie-0.1.1/omie/services/
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2096 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAltaDesagregacionesCP.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2096 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAltaDesagregacionesMC.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2156 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAltaEnergiasComprometidas.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2183 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAltaMessagesUmmElectricity.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2117 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAltaMessagesUmmOther.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1970 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAltaOfertasMD.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1969 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAltaOfertasMI.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2093 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAnulacionOfertasMD.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2150 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAnulacionOfertasMIAgente.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2147 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioAnulacionOfertasMIUnidad.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1902 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaDatosUsuario.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2138 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaDesagregacionesCP.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2138 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaDesagregacionesMC.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1837 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaFechaHora.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2708 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaMercados.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2042 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaOfertasMD.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2042 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaOfertasMI.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2036 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioConsultaUmm.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2015 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServicioDescargaREMIT.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4126 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServiciosConsultaDocumento.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5754 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServiciosConsultas.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5324 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServiciosConsultasAuxiliares.wsdl
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2748 2024-05-07 12:42:42.000000 omie-0.1.1/omie/services/ServiciosIdiomas.wsdl
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 14:14:51.986116 omie-0.1.1/omie/xsd/
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)   183600 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/Facturaev3_2_1.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    10953 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/InfoMercado.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    16966 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnotaciones.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3916 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMD.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4331 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMI.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3940 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionDesagregacionesCP.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3827 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionEjecucionesCBFFecha.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3556 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionEnergiaComprometida.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3942 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionExcedentesREDFecha.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4396 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionOfertaSesionMI.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4144 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionOfertasAgenteMI.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3772 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeAnulacionOfertasFechaMD.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     8198 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeCBF.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1645 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeCSV.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7355 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeCapacidadIntercambio.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     9665 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeCertificadosExportacion.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1436 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeConsultaDatosEnviados.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2084 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeConsultaFactura.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1746 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeConsultaUMM.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2370 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeDatosAgente.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5829 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeDeclExcedREDMD.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5966 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeDeclExcedREDMI.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7180 2024-05-07 12:42:42.000000 omie-0.1.1/omie/xsd/MensajeDesagregaciones.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6386 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeDesagregacionesCP.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6164 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeDesagregacionesMC.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6451 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeDesgloses.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7546 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeEjecCBF.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5116 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeEjecucionConsulta.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5668 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeEnergiasComprometidas.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6043 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeEnergiasTotales.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5741 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeExcedRED.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2212 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeFicherosNuevos.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3345 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeFicherosNuevosFact.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2860 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeFicherosNuevosLiq.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5228 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeHorasAnuladas.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5221 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeHorasAnuladasContinuo.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5185 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeImportesAcumulados.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     9800 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeOfertasMD.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    18381 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeOfertasMI.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4121 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeOfertasSubastasInterconexion.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5945 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajePrecios.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5358 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajePreciosContinuo.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3560 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajePreciosGasNatural.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7257 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajePrograma.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6209 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeProgramaContinuo.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2945 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeRetiradaDeclaracionesDefectoRE.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2920 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeRetiradaEjecucionesCBFDefecto.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2861 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeRetiradaOfertasDefectoMD.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1892 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeServicioDescargaREMIT.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7453 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/MensajeTransaccionesContinuo.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5730 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/REMITUMMCommonSchema_V1.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    11314 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/REMITUMMElectricitySchema_V2.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4894 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/REMITUMMOtherSchema_V1.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4771 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaAnulacionDesagregacionesCP.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4950 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaAnulacionRetiradaEjecucionesCBF.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4909 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaAnulacionRetiradaOfertas.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5055 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaAnulacionRetiradaRE.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    16083 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaConfiguracionConsulta.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    11060 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDatosUsuario.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6106 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDeclExcedRED.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6152 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDesagregaciones.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6023 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDesagregacionesCP.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6262 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDesagregacionesMC.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1869 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDescargaREMIT.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6090 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDesgloses.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3190 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaDirectorioConsultas.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5989 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaEjecCBF.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7196 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaEjecucionConsultaAnexo.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    14630 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaEjecucionConsultaEncolumnada.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1586 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaEjecucionConsultaPrograma.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5641 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaEnergiasComprometidas.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6015 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaExcedRED.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4770 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaFicherosNuevos.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4926 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaFicherosNuevosFact.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5317 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaFicherosNuevosLiq.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2532 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaListadoIdiomas.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2170 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaMensajesCortosActivos.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5915 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaOfertas.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    10557 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/RespuestaTiposFicheros.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    77065 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/eFactura_AEAT-CCI.xsd
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    48321 2024-05-07 12:42:43.000000 omie-0.1.1/omie/xsd/tiposOMEL.xsd
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 14:14:51.970116 omie-0.1.1/omie.egg-info/
--rw-r--r--   0 aorellana  (1000) aorellana  (1000)      268 2024-05-07 14:14:51.000000 omie-0.1.1/omie.egg-info/PKG-INFO
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4439 2024-05-07 14:14:51.000000 omie-0.1.1/omie.egg-info/SOURCES.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        1 2024-05-07 14:14:51.000000 omie-0.1.1/omie.egg-info/dependency_links.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       37 2024-05-07 14:14:51.000000 omie-0.1.1/omie.egg-info/entry_points.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-05-07 14:14:51.000000 omie-0.1.1/omie.egg-info/requires.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-05-07 14:14:51.000000 omie-0.1.1/omie.egg-info/top_level.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        4 2024-05-07 12:42:43.000000 omie-0.1.1/requirements.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       38 2024-05-07 14:14:51.986116 omie-0.1.1/setup.cfg
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1284 2024-05-07 14:13:42.000000 omie-0.1.1/setup.py
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-21 13:31:38.000000 omie-0.2.1/
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      278 2024-05-21 13:31:38.000000 omie-0.2.1/PKG-INFO
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-21 13:31:38.000000 omie-0.2.1/omie/
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-21 13:31:38.000000 omie-0.2.1/omie/xsd/
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     9665 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeCertificadosExportacion.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)   183600 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/Facturaev3_2_1.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    11314 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/REMITUMMElectricitySchema_V2.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3940 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6164 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeDesagregacionesMC.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3345 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeFicherosNuevosFact.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2860 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeFicherosNuevosLiq.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5228 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeHorasAnuladas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4894 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/REMITUMMOtherSchema_V1.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4771 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaAnulacionDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2532 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaListadoIdiomas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6152 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDesagregaciones.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5741 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeExcedRED.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5116 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeEjecucionConsulta.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2861 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeRetiradaOfertasDefectoMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6043 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeEnergiasTotales.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    10953 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/InfoMercado.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4396 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionOfertaSesionMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7196 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaEjecucionConsultaAnexo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6023 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7546 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeEjecCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    11060 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDatosUsuario.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    77065 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/eFactura_AEAT-CCI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5641 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaEnergiasComprometidas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    16083 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaConfiguracionConsulta.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    10557 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaTiposFicheros.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     8198 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     9800 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeOfertasMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4909 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaAnulacionRetiradaOfertas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    16966 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnotaciones.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2920 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeRetiradaEjecucionesCBFDefecto.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    14630 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaEjecucionConsultaEncolumnada.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5966 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeDeclExcedREDMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1645 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeCSV.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6015 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaExcedRED.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5829 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeDeclExcedREDMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3942 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionExcedentesREDFecha.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5730 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/REMITUMMCommonSchema_V1.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3916 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5945 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajePrecios.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1586 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaEjecucionConsultaPrograma.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6451 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeDesgloses.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6386 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6106 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDeclExcedRED.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5317 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaFicherosNuevosLiq.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5989 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaEjecCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3827 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionEjecucionesCBFFecha.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    48321 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/tiposOMEL.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1869 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDescargaREMIT.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6209 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeProgramaContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2370 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeDatosAgente.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6262 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDesagregacionesMC.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5668 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeEnergiasComprometidas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7180 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeDesagregaciones.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3560 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajePreciosGasNatural.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4770 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaFicherosNuevos.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4331 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2170 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaMensajesCortosActivos.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7453 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeTransaccionesContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7355 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeCapacidadIntercambio.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4121 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeOfertasSubastasInterconexion.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2212 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeFicherosNuevos.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5221 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeHorasAnuladasContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5915 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaOfertas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4950 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaAnulacionRetiradaEjecucionesCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3190 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDirectorioConsultas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1746 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeConsultaUMM.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6090 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaDesgloses.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4926 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaFicherosNuevosFact.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    18381 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeOfertasMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1436 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeConsultaDatosEnviados.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5055 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/RespuestaAnulacionRetiradaRE.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2084 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeConsultaFactura.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7257 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajePrograma.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1892 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeServicioDescargaREMIT.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3772 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionOfertasFechaMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3556 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionEnergiaComprometida.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5358 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajePreciosContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2945 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeRetiradaDeclaracionesDefectoRE.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5185 2024-05-07 12:42:43.000000 omie-0.2.1/omie/xsd/MensajeImportesAcumulados.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4144 2024-05-07 12:42:42.000000 omie-0.2.1/omie/xsd/MensajeAnulacionOfertasAgenteMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     8712 2024-05-16 07:08:04.000000 omie-0.2.1/omie/omie.py
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-21 13:31:38.000000 omie-0.2.1/omie/services/
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2147 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAnulacionOfertasMIUnidad.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2708 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaMercados.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2015 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioDescargaREMIT.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2093 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAnulacionOfertasMD.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1837 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaFechaHora.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2138 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaDesagregacionesMC.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2042 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaOfertasMD.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5324 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServiciosConsultasAuxiliares.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2150 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAnulacionOfertasMIAgente.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2156 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAltaEnergiasComprometidas.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4126 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServiciosConsultaDocumento.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2036 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaUmm.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2096 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAltaDesagregacionesCP.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2138 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaDesagregacionesCP.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1970 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAltaOfertasMD.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5754 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServiciosConsultas.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1902 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaDatosUsuario.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1969 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAltaOfertasMI.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2183 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAltaMessagesUmmElectricity.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2748 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServiciosIdiomas.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2042 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioConsultaOfertasMI.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2117 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAltaMessagesUmmOther.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2096 2024-05-07 12:42:42.000000 omie-0.2.1/omie/services/ServicioAltaDesagregacionesMC.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       55 2024-05-07 12:42:42.000000 omie-0.2.1/omie/__init__.py
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      230 2024-05-07 12:42:42.000000 omie-0.2.1/README.md
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       24 2024-05-07 14:22:06.000000 omie-0.2.1/MANIFEST.in
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        4 2024-05-09 12:49:07.000000 omie-0.2.1/requirements.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       38 2024-05-21 13:31:38.000000 omie-0.2.1/setup.cfg
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1284 2024-05-21 13:28:10.000000 omie-0.2.1/setup.py
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-21 13:31:38.000000 omie-0.2.1/omie.egg-info/
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        1 2024-05-21 13:31:38.000000 omie-0.2.1/omie.egg-info/dependency_links.txt
+-rw-r--r--   0 aorellana  (1000) aorellana  (1000)      278 2024-05-21 13:31:38.000000 omie-0.2.1/omie.egg-info/PKG-INFO
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-05-21 13:31:38.000000 omie-0.2.1/omie.egg-info/requires.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-05-21 13:31:38.000000 omie-0.2.1/omie.egg-info/top_level.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       52 2024-05-21 13:31:38.000000 omie-0.2.1/omie.egg-info/entry_points.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4439 2024-05-21 13:31:38.000000 omie-0.2.1/omie.egg-info/SOURCES.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `omie-0.1.1/omie/services/ServicioAltaDesagregacionesCP.wsdl` & `omie-0.2.1/omie/services/ServicioAltaDesagregacionesCP.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAltaDesagregacionesMC.wsdl` & `omie-0.2.1/omie/services/ServicioAltaDesagregacionesMC.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAltaEnergiasComprometidas.wsdl` & `omie-0.2.1/omie/services/ServicioAltaEnergiasComprometidas.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAltaMessagesUmmElectricity.wsdl` & `omie-0.2.1/omie/services/ServicioAltaMessagesUmmElectricity.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAltaMessagesUmmOther.wsdl` & `omie-0.2.1/omie/services/ServicioAltaMessagesUmmOther.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAltaOfertasMD.wsdl` & `omie-0.2.1/omie/services/ServicioAltaOfertasMD.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAltaOfertasMI.wsdl` & `omie-0.2.1/omie/services/ServicioAltaOfertasMI.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAnulacionOfertasMD.wsdl` & `omie-0.2.1/omie/services/ServicioAnulacionOfertasMD.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAnulacionOfertasMIAgente.wsdl` & `omie-0.2.1/omie/services/ServicioAnulacionOfertasMIAgente.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioAnulacionOfertasMIUnidad.wsdl` & `omie-0.2.1/omie/services/ServicioAnulacionOfertasMIUnidad.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaDatosUsuario.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaDatosUsuario.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaDesagregacionesCP.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaDesagregacionesCP.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaDesagregacionesMC.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaDesagregacionesMC.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaFechaHora.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaFechaHora.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaMercados.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaMercados.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaOfertasMD.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaOfertasMD.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaOfertasMI.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaOfertasMI.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioConsultaUmm.wsdl` & `omie-0.2.1/omie/services/ServicioConsultaUmm.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServicioDescargaREMIT.wsdl` & `omie-0.2.1/omie/services/ServicioDescargaREMIT.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServiciosConsultaDocumento.wsdl` & `omie-0.2.1/omie/services/ServiciosConsultaDocumento.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServiciosConsultas.wsdl` & `omie-0.2.1/omie/services/ServiciosConsultas.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServiciosConsultasAuxiliares.wsdl` & `omie-0.2.1/omie/services/ServiciosConsultasAuxiliares.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/services/ServiciosIdiomas.wsdl` & `omie-0.2.1/omie/services/ServiciosIdiomas.wsdl`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/Facturaev3_2_1.xsd` & `omie-0.2.1/omie/xsd/Facturaev3_2_1.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/InfoMercado.xsd` & `omie-0.2.1/omie/xsd/InfoMercado.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnotaciones.xsd` & `omie-0.2.1/omie/xsd/MensajeAnotaciones.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMD.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMD.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMI.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionDeclaracionesREFechaMI.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionDesagregacionesCP.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionDesagregacionesCP.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionEjecucionesCBFFecha.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionEjecucionesCBFFecha.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionEnergiaComprometida.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionEnergiaComprometida.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionExcedentesREDFecha.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionExcedentesREDFecha.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionOfertaSesionMI.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionOfertaSesionMI.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionOfertasAgenteMI.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionOfertasAgenteMI.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeAnulacionOfertasFechaMD.xsd` & `omie-0.2.1/omie/xsd/MensajeAnulacionOfertasFechaMD.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeCBF.xsd` & `omie-0.2.1/omie/xsd/MensajeCBF.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeCSV.xsd` & `omie-0.2.1/omie/xsd/MensajeCSV.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeCapacidadIntercambio.xsd` & `omie-0.2.1/omie/xsd/MensajeCapacidadIntercambio.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeCertificadosExportacion.xsd` & `omie-0.2.1/omie/xsd/MensajeCertificadosExportacion.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeConsultaDatosEnviados.xsd` & `omie-0.2.1/omie/xsd/MensajeConsultaDatosEnviados.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeConsultaFactura.xsd` & `omie-0.2.1/omie/xsd/MensajeConsultaFactura.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeConsultaUMM.xsd` & `omie-0.2.1/omie/xsd/MensajeConsultaUMM.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeDatosAgente.xsd` & `omie-0.2.1/omie/xsd/MensajeDatosAgente.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeDeclExcedREDMD.xsd` & `omie-0.2.1/omie/xsd/MensajeDeclExcedREDMD.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeDeclExcedREDMI.xsd` & `omie-0.2.1/omie/xsd/MensajeDeclExcedREDMI.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeDesagregaciones.xsd` & `omie-0.2.1/omie/xsd/MensajeDesagregaciones.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeDesagregacionesCP.xsd` & `omie-0.2.1/omie/xsd/MensajeDesagregacionesCP.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeDesagregacionesMC.xsd` & `omie-0.2.1/omie/xsd/MensajeDesagregacionesMC.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeDesgloses.xsd` & `omie-0.2.1/omie/xsd/MensajeDesgloses.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeEjecCBF.xsd` & `omie-0.2.1/omie/xsd/MensajeEjecCBF.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeEjecucionConsulta.xsd` & `omie-0.2.1/omie/xsd/MensajeEjecucionConsulta.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeEnergiasComprometidas.xsd` & `omie-0.2.1/omie/xsd/MensajeEnergiasComprometidas.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeEnergiasTotales.xsd` & `omie-0.2.1/omie/xsd/MensajeEnergiasTotales.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeExcedRED.xsd` & `omie-0.2.1/omie/xsd/MensajeExcedRED.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeFicherosNuevos.xsd` & `omie-0.2.1/omie/xsd/MensajeFicherosNuevos.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeFicherosNuevosFact.xsd` & `omie-0.2.1/omie/xsd/MensajeFicherosNuevosFact.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeFicherosNuevosLiq.xsd` & `omie-0.2.1/omie/xsd/MensajeFicherosNuevosLiq.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeHorasAnuladas.xsd` & `omie-0.2.1/omie/xsd/MensajeHorasAnuladas.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeHorasAnuladasContinuo.xsd` & `omie-0.2.1/omie/xsd/MensajeHorasAnuladasContinuo.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeImportesAcumulados.xsd` & `omie-0.2.1/omie/xsd/MensajeImportesAcumulados.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeOfertasMD.xsd` & `omie-0.2.1/omie/xsd/MensajeOfertasMD.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeOfertasMI.xsd` & `omie-0.2.1/omie/xsd/MensajeOfertasMI.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeOfertasSubastasInterconexion.xsd` & `omie-0.2.1/omie/xsd/MensajeOfertasSubastasInterconexion.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajePrecios.xsd` & `omie-0.2.1/omie/xsd/MensajePrecios.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajePreciosContinuo.xsd` & `omie-0.2.1/omie/xsd/MensajePreciosContinuo.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajePreciosGasNatural.xsd` & `omie-0.2.1/omie/xsd/MensajePreciosGasNatural.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajePrograma.xsd` & `omie-0.2.1/omie/xsd/MensajePrograma.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeProgramaContinuo.xsd` & `omie-0.2.1/omie/xsd/MensajeProgramaContinuo.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeRetiradaDeclaracionesDefectoRE.xsd` & `omie-0.2.1/omie/xsd/MensajeRetiradaDeclaracionesDefectoRE.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeRetiradaEjecucionesCBFDefecto.xsd` & `omie-0.2.1/omie/xsd/MensajeRetiradaEjecucionesCBFDefecto.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeRetiradaOfertasDefectoMD.xsd` & `omie-0.2.1/omie/xsd/MensajeRetiradaOfertasDefectoMD.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeServicioDescargaREMIT.xsd` & `omie-0.2.1/omie/xsd/MensajeServicioDescargaREMIT.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/MensajeTransaccionesContinuo.xsd` & `omie-0.2.1/omie/xsd/MensajeTransaccionesContinuo.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/REMITUMMCommonSchema_V1.xsd` & `omie-0.2.1/omie/xsd/REMITUMMCommonSchema_V1.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/REMITUMMElectricitySchema_V2.xsd` & `omie-0.2.1/omie/xsd/REMITUMMElectricitySchema_V2.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/REMITUMMOtherSchema_V1.xsd` & `omie-0.2.1/omie/xsd/REMITUMMOtherSchema_V1.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaAnulacionDesagregacionesCP.xsd` & `omie-0.2.1/omie/xsd/RespuestaAnulacionDesagregacionesCP.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaAnulacionRetiradaEjecucionesCBF.xsd` & `omie-0.2.1/omie/xsd/RespuestaAnulacionRetiradaEjecucionesCBF.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaAnulacionRetiradaOfertas.xsd` & `omie-0.2.1/omie/xsd/RespuestaAnulacionRetiradaOfertas.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaAnulacionRetiradaRE.xsd` & `omie-0.2.1/omie/xsd/RespuestaAnulacionRetiradaRE.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaConfiguracionConsulta.xsd` & `omie-0.2.1/omie/xsd/RespuestaConfiguracionConsulta.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDatosUsuario.xsd` & `omie-0.2.1/omie/xsd/RespuestaDatosUsuario.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDeclExcedRED.xsd` & `omie-0.2.1/omie/xsd/RespuestaDeclExcedRED.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDesagregaciones.xsd` & `omie-0.2.1/omie/xsd/RespuestaDesagregaciones.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDesagregacionesCP.xsd` & `omie-0.2.1/omie/xsd/RespuestaDesagregacionesCP.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDesagregacionesMC.xsd` & `omie-0.2.1/omie/xsd/RespuestaDesagregacionesMC.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDescargaREMIT.xsd` & `omie-0.2.1/omie/xsd/RespuestaDescargaREMIT.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDesgloses.xsd` & `omie-0.2.1/omie/xsd/RespuestaDesgloses.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaDirectorioConsultas.xsd` & `omie-0.2.1/omie/xsd/RespuestaDirectorioConsultas.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaEjecCBF.xsd` & `omie-0.2.1/omie/xsd/RespuestaEjecCBF.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaEjecucionConsultaAnexo.xsd` & `omie-0.2.1/omie/xsd/RespuestaEjecucionConsultaAnexo.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaEjecucionConsultaEncolumnada.xsd` & `omie-0.2.1/omie/xsd/RespuestaEjecucionConsultaEncolumnada.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaEjecucionConsultaPrograma.xsd` & `omie-0.2.1/omie/xsd/RespuestaEjecucionConsultaPrograma.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaEnergiasComprometidas.xsd` & `omie-0.2.1/omie/xsd/RespuestaEnergiasComprometidas.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaExcedRED.xsd` & `omie-0.2.1/omie/xsd/RespuestaExcedRED.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaFicherosNuevos.xsd` & `omie-0.2.1/omie/xsd/RespuestaFicherosNuevos.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaFicherosNuevosFact.xsd` & `omie-0.2.1/omie/xsd/RespuestaFicherosNuevosFact.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaFicherosNuevosLiq.xsd` & `omie-0.2.1/omie/xsd/RespuestaFicherosNuevosLiq.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaListadoIdiomas.xsd` & `omie-0.2.1/omie/xsd/RespuestaListadoIdiomas.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaMensajesCortosActivos.xsd` & `omie-0.2.1/omie/xsd/RespuestaMensajesCortosActivos.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaOfertas.xsd` & `omie-0.2.1/omie/xsd/RespuestaOfertas.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/RespuestaTiposFicheros.xsd` & `omie-0.2.1/omie/xsd/RespuestaTiposFicheros.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/eFactura_AEAT-CCI.xsd` & `omie-0.2.1/omie/xsd/eFactura_AEAT-CCI.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie/xsd/tiposOMEL.xsd` & `omie-0.2.1/omie/xsd/tiposOMEL.xsd`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/omie.egg-info/SOURCES.txt` & `omie-0.2.1/omie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omie-0.1.1/setup.py` & `omie-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if os.path.exists(self.build_base):
             print("Cleaning {} dir".format(self.build_base))
             shutil.rmtree(self.build_base)
 
 
 setup(
     name='omie',
-    version='0.1.1',
+    version='0.2.1',
     description='Libreria de interacción con OMIE',
     author='Adrià Orellana',
     author_email='aorellana@gisce.net',
     url='http://www.gisce.net',
     license='General Public Licence 2',
     long_description='''Long description''',
     provides=['omie'],
```

