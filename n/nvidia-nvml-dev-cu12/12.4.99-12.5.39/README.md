# Comparing `tmp/nvidia_nvml_dev_cu12-12.4.99-py3-none-win_amd64.whl.zip` & `tmp/nvidia_nvml_dev_cu12-12.5.39-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,11 @@
-Zip file size: 119718 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 01:10 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/include/__init__.py
--rw-r--r--  2.0 unx   589454 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/include/nvml.h
--rw-r--r--  2.0 unx    95280 b- defN 24-Feb-28 01:10 nvidia/nvml_dev/lib/x64/nvml.lib
--rw-r--r--  2.0 unx    59262 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/License.txt
--rw-r--r--  2.0 unx     1504 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      886 b- defN 24-Feb-28 01:10 nvidia_nvml_dev_cu12-12.4.99.dist-info/RECORD
-10 files, 746491 bytes uncompressed, 118176 bytes compressed:  84.2%
+Zip file size: 104874 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 23:54 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 23:54 nvidia/nvml_dev/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-16 23:54 nvidia/nvml_dev/include/__init__.py
+-rw-r--r--  2.0 unx   595956 b- defN 24-Apr-16 23:54 nvidia/nvml_dev/include/nvml.h
+-rw-r--r--  2.0 unx    59262 b- defN 24-Apr-16 23:54 nvidia_nvml_dev_cu12-12.5.39.dist-info/License.txt
+-rw-r--r--  2.0 unx     1507 b- defN 24-Apr-16 23:54 nvidia_nvml_dev_cu12-12.5.39.dist-info/METADATA
+-rw-r--r--  2.0 unx      109 b- defN 24-Apr-16 23:54 nvidia_nvml_dev_cu12-12.5.39.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-16 23:54 nvidia_nvml_dev_cu12-12.5.39.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      797 b- defN 24-Apr-16 23:54 nvidia_nvml_dev_cu12-12.5.39.dist-info/RECORD
+9 files, 657638 bytes uncompressed, 103472 bytes compressed:  84.3%
```

## zipnote {}

```diff
@@ -6,26 +6,23 @@
 
 Filename: nvidia/nvml_dev/include/__init__.py
 Comment: 
 
 Filename: nvidia/nvml_dev/include/nvml.h
 Comment: 
 
-Filename: nvidia/nvml_dev/lib/x64/nvml.lib
+Filename: nvidia_nvml_dev_cu12-12.5.39.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/License.txt
+Filename: nvidia_nvml_dev_cu12-12.5.39.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/METADATA
+Filename: nvidia_nvml_dev_cu12-12.5.39.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/WHEEL
+Filename: nvidia_nvml_dev_cu12-12.5.39.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/top_level.txt
-Comment: 
-
-Filename: nvidia_nvml_dev_cu12-12.4.99.dist-info/RECORD
+Filename: nvidia_nvml_dev_cu12-12.5.39.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia/nvml_dev/include/nvml.h

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 1993-2023 NVIDIA Corporation.  All rights reserved.
+ * Copyright 1993-2024 NVIDIA Corporation.  All rights reserved.
  *
  * NOTICE TO USER:
  *
  * This source code is subject to NVIDIA ownership rights under U.S. and
  * international Copyright laws.  Users and possessors of this source code
  * are hereby granted a nonexclusive, royalty-free license to use this code
  * in individual and commercial software.
@@ -88,14 +88,16 @@
     #else
         #define DECLDIR
     #endif
 #else
     #define DECLDIR
 #endif
 
+    #define NVML_MCDM_SUPPORT
+
 /**
  * NVML API versioning support
  */
 #define NVML_API_VERSION            12
 #define NVML_API_VERSION_STR        "12"
 /**
  * Defining NVML_NO_UNVERSIONED_FUNC_DEFS will disable "auto upgrading" of APIs.
@@ -118,14 +120,15 @@
     #define nvmlDeviceGetGraphicsRunningProcesses       nvmlDeviceGetGraphicsRunningProcesses_v3
     #define nvmlDeviceGetMPSComputeRunningProcesses     nvmlDeviceGetMPSComputeRunningProcesses_v3
     #define nvmlBlacklistDeviceInfo_t                   nvmlExcludedDeviceInfo_t
     #define nvmlGetBlacklistDeviceCount                 nvmlGetExcludedDeviceCount
     #define nvmlGetBlacklistDeviceInfoByIndex           nvmlGetExcludedDeviceInfoByIndex
     #define nvmlDeviceGetGpuInstancePossiblePlacements  nvmlDeviceGetGpuInstancePossiblePlacements_v2
     #define nvmlVgpuInstanceGetLicenseInfo              nvmlVgpuInstanceGetLicenseInfo_v2
+    #define nvmlDeviceGetDriverModel                    nvmlDeviceGetDriverModel_v2
 #endif // #ifndef NVML_NO_UNVERSIONED_FUNC_DEFS
 
 #define NVML_STRUCT_VERSION(data, ver) (unsigned int)(sizeof(nvml ## data ## _v ## ver ## _t) | \
                                                       (ver << 24U))
 
 /***************************************************************************************************/
 /** @defgroup nvmlDeviceStructs Device Structs
@@ -757,14 +760,16 @@
                                                   // can be throttled below base clock
     NVML_TEMPERATURE_THRESHOLD_ACOUSTIC_MIN  = 4, // Minimum GPU Temperature that can be
                                                   // set as acoustic threshold
     NVML_TEMPERATURE_THRESHOLD_ACOUSTIC_CURR = 5, // Current temperature that is set as
                                                   // acoustic threshold.
     NVML_TEMPERATURE_THRESHOLD_ACOUSTIC_MAX  = 6, // Maximum GPU temperature that can be
                                                   // set as acoustic threshold.
+    NVML_TEMPERATURE_THRESHOLD_GPS_CURR      = 7, // Current temperature that is set as
+                                                  // gps threshold.
     // Keep this last
     NVML_TEMPERATURE_THRESHOLD_COUNT
 } nvmlTemperatureThresholds_t;
 
 /**
  * Temperature sensors.
  */
@@ -933,16 +938,17 @@
  * Driver models.
  *
  * Windows only.
  */
 
 typedef enum nvmlDriverModel_enum
 {
-    NVML_DRIVER_WDDM = 0,       //!< WDDM driver model -- GPU treated as a display device
-    NVML_DRIVER_WDM = 1        //!< WDM (TCC) model (recommended) -- GPU treated as a generic device
+    NVML_DRIVER_WDDM      = 0,       //!< WDDM driver model -- GPU treated as a display device
+    NVML_DRIVER_WDM       = 1,       //!< WDM (TCC) model (deprecated) -- GPU treated as a generic compute device
+    NVML_DRIVER_MCDM      = 2        //!< MCDM driver model -- GPU treated as a Microsoft compute device
 } nvmlDriverModel_t;
 
 #define NVML_MAX_GPU_PERF_PSTATES 16
 
 /**
  * Allowed PStates.
  */
@@ -964,14 +970,31 @@
     NVML_PSTATE_13              = 13,      //!< Performance state 13
     NVML_PSTATE_14              = 14,      //!< Performance state 14
     NVML_PSTATE_15              = 15,      //!< Performance state 15 -- Minimum Performance
     NVML_PSTATE_UNKNOWN         = 32       //!< Unknown performance state
 } nvmlPstates_t;
 
 /**
+ * Clock offset info.
+ */
+typedef struct
+{
+    unsigned int version; //!< The version number of this struct
+    nvmlClockType_t type;
+    nvmlPstates_t pstate;
+    int clockOffsetMHz;
+    int minClockOffsetMHz;
+    int maxClockOffsetMHz;
+} nvmlClockOffset_v1_t;
+
+typedef nvmlClockOffset_v1_t nvmlClockOffset_t;
+
+#define nvmlClockOffset_v1 NVML_STRUCT_VERSION(ClockOffset, 1)
+
+/**
  * GPU Operation Mode
  *
  * GOM allows to reduce power usage and optimize GPU throughput by disabling GPU features.
  *
  * Each GOM is designed to meet specific user needs.
  */
 typedef enum nvmlGom_enum
@@ -1621,14 +1644,16 @@
 #define NVML_DEVICE_ARCH_PASCAL    4 // Devices based on the NVIDIA Pascal architecture
 #define NVML_DEVICE_ARCH_VOLTA     5 // Devices based on the NVIDIA Volta architecture
 #define NVML_DEVICE_ARCH_TURING    6 // Devices based on the NVIDIA Turing architecture
 #define NVML_DEVICE_ARCH_AMPERE    7 // Devices based on the NVIDIA Ampere architecture
 #define NVML_DEVICE_ARCH_ADA       8 // Devices based on the NVIDIA Ada architecture
 #define NVML_DEVICE_ARCH_HOPPER    9 // Devices based on the NVIDIA Hopper architecture
 
+#define NVML_DEVICE_ARCH_T23X      11 // Devices based on NVIDIA Orin architecture
+
 #define NVML_DEVICE_ARCH_UNKNOWN   0xffffffff // Anything else, presumably something newer
 
 typedef unsigned int nvmlDeviceArchitecture_t;
 
 /**
  * PCI bus types
  */
@@ -2012,18 +2037,22 @@
  * These fields are supported on Ada and later architectures and supersedes \ref nvmlDeviceGetTemperatureThreshold.
  */
 #define NVML_FI_DEV_TEMPERATURE_SHUTDOWN_TLIMIT       193 //!< T.Limit temperature after which GPU may shut down for HW protection
 #define NVML_FI_DEV_TEMPERATURE_SLOWDOWN_TLIMIT       194 //!< T.Limit temperature after which GPU may begin HW slowdown
 #define NVML_FI_DEV_TEMPERATURE_MEM_MAX_TLIMIT        195 //!< T.Limit temperature after which GPU may begin SW slowdown due to memory temperature
 #define NVML_FI_DEV_TEMPERATURE_GPU_MAX_TLIMIT        196 //!< T.Limit temperature after which GPU may be throttled below base clock
 
-#define NVML_FI_DEV_IS_MIG_MODE_INDEPENDENT_MIG_QUERY_CAPABLE   199 //!< MIG mode independent, MIG query capable device. 1=yes. 0=no.
+#define NVML_FI_DEV_PCIE_COUNT_TX_BYTES               197 //!< PCIe transmit bytes. Value can be wrapped.
+#define NVML_FI_DEV_PCIE_COUNT_RX_BYTES               198 //!< PCIe receive bytes. Value can be wrapped.
+
+#define NVML_FI_DEV_NVLINK_GET_POWER_THRESHOLD_MAX    199 //!< Max Nvlink Power Threshold. See NVML_FI_DEV_NVLINK_GET_POWER_THRESHOLD
 
-#define NVML_FI_MAX                                   200 //!< One greater than the largest field ID defined above
+#define NVML_FI_DEV_IS_MIG_MODE_INDEPENDENT_MIG_QUERY_CAPABLE   200 //!< MIG mode independent, MIG query capable device. 1=yes. 0=no.
 
+#define NVML_FI_MAX                                       223 //!< One greater than the largest field ID defined above
 /**
  * Information for a Field Value Sample
  */
 typedef struct nvmlFieldValue_st
 {
     unsigned int fieldId;       //!< ID of the NVML field to retrieve. This must be set before any call that uses this struct. See the constants starting with NVML_FI_ above.
     unsigned int scopeId;       //!< Scope ID can represent data used by NVML depending on fieldId's context. For example, for NVLink throughput counter data, scopeId can represent linkId.
@@ -4538,34 +4567,35 @@
  *         - \ref NVML_ERROR_NOT_SUPPORTED     if the device does not have a fan
  *         - \ref NVML_ERROR_GPU_IS_LOST       if the target GPU has fallen off the bus or is otherwise inaccessible
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlDeviceGetNumFans(nvmlDevice_t device, unsigned int *numFans);
 
 /**
- * Retrieves the current temperature readings for the device, in degrees C.
- *
- * For all products.
- *
- * See \ref nvmlTemperatureSensors_t for details on available temperature sensors.
- *
- * @param device                               The identifier of the target device
- * @param sensorType                           Flag that indicates which sensor reading to retrieve
- * @param temp                                 Reference in which to return the temperature reading
- *
- * @return
- *         - \ref NVML_SUCCESS                 if \a temp has been set
- *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
- *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid, \a sensorType is invalid or \a temp is NULL
- *         - \ref NVML_ERROR_NOT_SUPPORTED     if the device does not have the specified sensor
- *         - \ref NVML_ERROR_GPU_IS_LOST       if the target GPU has fallen off the bus or is otherwise inaccessible
- *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
- */
+   * Retrieves the current temperature readings for the device, in degrees C.
+   *
+   * For all products.
+   *
+   * See \ref nvmlTemperatureSensors_t for details on available temperature sensors.
+   *
+   * @param device                               The identifier of the target device
+   * @param sensorType                           Flag that indicates which sensor reading to retrieve
+   * @param temp                                 Reference in which to return the temperature reading
+   *
+   * @return
+   *         - \ref NVML_SUCCESS                 if \a temp has been set
+   *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
+   *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid, \a sensorType is invalid or \a temp is NULL
+   *         - \ref NVML_ERROR_NOT_SUPPORTED     if the device does not have the specified sensor
+   *         - \ref NVML_ERROR_GPU_IS_LOST       if the target GPU has fallen off the bus or is otherwise inaccessible
+   *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
+   */
 nvmlReturn_t DECLDIR nvmlDeviceGetTemperature(nvmlDevice_t device, nvmlTemperatureSensors_t sensorType, unsigned int *temp);
 
+
 /**
  * Retrieves the temperature threshold for the GPU with the specified threshold type in degrees C.
  *
  * For Kepler &tm; or newer fully supported devices.
  *
  * See \ref nvmlTemperatureThresholds_t for details on available temperature thresholds.
  *
@@ -4811,14 +4841,60 @@
  *         - \ref NVML_ERROR_NOT_SUPPORTED     if the device does not support this feature
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlDeviceGetMemClkMinMaxVfOffset(nvmlDevice_t device,
                                                        int *minOffset, int *maxOffset);
 
 /**
+ * Retrieve min, max and current clock offset of some clock domain for a given PState
+ *
+ * For Maxwell &tm; or newer fully supported devices.
+ *
+ * Note: \ref nvmlDeviceGetGpcClkVfOffset, \ref nvmlDeviceGetMemClkVfOffset, \ref nvmlDeviceGetGpcClkMinMaxVfOffset and
+ *       \ref nvmlDeviceGetMemClkMinMaxVfOffset will be deprecated in a future release.
+         Use \ref nvmlDeviceGetClockOffsets instead.
+ *
+ * @param device                               The identifier of the target device
+ * @param info                                 Structure specifying the clock type (input) and the pstate (input)
+ *                                             retrieved clock offset value (output), min clock offset (output)
+ *                                             and max clock offset (output)
+ *
+ * @return
+ *         - \ref NVML_SUCCESS                         if everything worked
+ *         - \ref NVML_ERROR_UNINITIALIZED             if the library has not been successfully initialized
+ *         - \ref NVML_ERROR_INVALID_ARGUMENT          if \a device, \a type or \a pstate are invalid or both
+ *                                                             \a minClockOffsetMHz and \a maxClockOffsetMHz are NULL
+ *         - \ref NVML_ERROR_ARGUMENT_VERSION_MISMATCH if the provided version is invalid/unsupported
+ *         - \ref NVML_ERROR_NOT_SUPPORTED             if the device does not support this feature
+ */
+nvmlReturn_t DECLDIR nvmlDeviceGetClockOffsets(nvmlDevice_t device, nvmlClockOffset_t *info);
+
+/**
+ * Control current clock offset of some clock domain for a given PState
+ *
+ * For Maxwell &tm; or newer fully supported devices.
+ *
+ * Requires privileged user.
+ *
+ * @param device                               The identifier of the target device
+ * @param info                                 Structure specifying the clock type (input), the pstate (input)
+ *                                             and clock offset value (input)
+ *
+ * @return
+ *         - \ref NVML_SUCCESS                         if everything worked
+ *         - \ref NVML_ERROR_UNINITIALIZED             if the library has not been successfully initialized
+ *         - \ref NVML_ERROR_NO_PERMISSION             if the user doesn't have permission to perform this operation
+ *         - \ref NVML_ERROR_INVALID_ARGUMENT          if \a device, \a type or \a pstate are invalid or both
+ *                                                             \a clockOffsetMHz is out of allowed range.
+ *         - \ref NVML_ERROR_ARGUMENT_VERSION_MISMATCH if the provided version is invalid/unsupported
+ *         - \ref NVML_ERROR_NOT_SUPPORTED             if the device does not support this feature
+ */
+nvmlReturn_t DECLDIR nvmlDeviceSetClockOffsets(nvmlDevice_t device, nvmlClockOffset_t *info);
+
+/**
  * This API has been deprecated.
  *
  * Retrieves the power management mode associated with this device.
  *
  * For products from the Fermi family.
  *     - Requires \a NVML_INFOROM_POWER version 3.0 or higher.
  *
@@ -5517,19 +5593,19 @@
 *         - \ref NVML_ERROR_UNKNOWN            on any unexpected error
 */
 nvmlReturn_t DECLDIR nvmlDeviceGetFBCSessions(nvmlDevice_t device, unsigned int *sessionCount, nvmlFBCSessionInfo_t *sessionInfo);
 
 /**
  * Retrieves the current and pending driver model for the device.
  *
- * For Fermi &tm; or newer fully supported devices.
+ * For Kepler &tm; or newer fully supported devices.
  * For windows only.
  *
- * On Windows platforms the device driver can run in either WDDM or WDM (TCC) mode. If a display is attached
- * to the device it must run in WDDM mode. TCC mode is preferred if a display is not attached.
+ * On Windows platforms the device driver can run in either WDDM, MCDM or WDM (TCC) modes. If a display is attached
+ * to the device it must run in WDDM mode. MCDM mode is preferred if a display is not attached. TCC mode is deprecated.
  *
  * See \ref nvmlDriverModel_t for details on available driver models.
  *
  * @param device                               The identifier of the target device
  * @param current                              Reference in which to return the current driver model
  * @param pending                              Reference in which to return the pending driver model
  *
@@ -5537,17 +5613,17 @@
  *         - \ref NVML_SUCCESS                 if either \a current and/or \a pending have been set
  *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
  *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid or both \a current and \a pending are NULL
  *         - \ref NVML_ERROR_NOT_SUPPORTED     if the platform is not windows
  *         - \ref NVML_ERROR_GPU_IS_LOST       if the target GPU has fallen off the bus or is otherwise inaccessible
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  *
- * @see nvmlDeviceSetDriverModel()
+ * @see nvmlDeviceSetDriverModel_v2()
  */
-nvmlReturn_t DECLDIR nvmlDeviceGetDriverModel(nvmlDevice_t device, nvmlDriverModel_t *current, nvmlDriverModel_t *pending);
+nvmlReturn_t DECLDIR nvmlDeviceGetDriverModel_v2(nvmlDevice_t device, nvmlDriverModel_t *current, nvmlDriverModel_t *pending);
 
 /**
  * Get VBIOS version of the device.
  *
  * For all products.
  *
  * The VBIOS version may change from time to time. It will not exceed 32 characters in length
@@ -5670,15 +5746,15 @@
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  *
  * @see \ref nvmlSystemGetProcessName
  */
 nvmlReturn_t DECLDIR nvmlDeviceGetGraphicsRunningProcesses_v3(nvmlDevice_t device, unsigned int *infoCount, nvmlProcessInfo_t *infos);
 
 /**
- * Get information about processes with a MPS compute context on a device
+ * Get information about processes with a Multi-Process Service (MPS) compute context on a device
  *
  * For Volta &tm; or newer fully supported devices.
  *
  * This function returns information only about compute running processes (e.g. CUDA application which have
  * active context) utilizing MPS. Any graphics applications (e.g. using OpenGL, DirectX) won't be listed by
  * this function.
  *
@@ -6223,14 +6299,72 @@
  *         - \ref NVML_ERROR_NOT_SUPPORTED     if this query is not supported by the device
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlSystemGetConfComputeKeyRotationThresholdInfo(
                           nvmlConfComputeGetKeyRotationThresholdInfo_t *pKeyRotationThrInfo);
 
 /**
+ * Set Conf Computing Unprotected Memory Size.
+ *
+ * For Ampere &tm; or newer fully supported devices.
+ * Supported on Linux, Windows TCC.
+ *
+ * @param device                               Device Handle
+ * @param sizeKiB                              Unprotected Memory size to be set in KiB
+ *
+ * @return
+ *         - \ref NVML_SUCCESS                 if \a sizeKiB successfully set
+ *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
+ *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid
+ *         - \ref NVML_ERROR_NOT_SUPPORTED     if this query is not supported by the device
+ */
+nvmlReturn_t DECLDIR nvmlDeviceSetConfComputeUnprotectedMemSize(nvmlDevice_t device, unsigned long long sizeKiB);
+
+/**
+ * Set Conf Computing GPUs ready state.
+ *
+ * For Ampere &tm; or newer fully supported devices.
+ * Supported on Linux, Windows TCC.
+ *
+ * @param isAcceptingWork                      GPU accepting new work, NVML_CC_ACCEPTING_CLIENT_REQUESTS_TRUE or
+ *                                             NVML_CC_ACCEPTING_CLIENT_REQUESTS_FALSE
+ *
+ * return
+ *         - \ref NVML_SUCCESS                 if \a current GPUs ready state is successfully set
+ *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
+ *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a isAcceptingWork is invalid
+ *         - \ref NVML_ERROR_NOT_SUPPORTED     if this query is not supported by the device
+ */
+nvmlReturn_t DECLDIR nvmlSystemSetConfComputeGpusReadyState(unsigned int isAcceptingWork);
+
+/**
+ * Set Conf Computing key rotation threshold. 
+ *
+ * %HOPPER_OR_NEWER%
+ * Supported on Linux, Windows TCC.
+ *
+ * This function is to set the confidential compute key rotation threshold parameters.
+ * @ref pKeyRotationThrInfo->maxAttackerAdvantage should be in the range from 
+ * NVML_CC_KEY_ROTATION_THRESHOLD_ATTACKER_ADVANTAGE_MIN to NVML_CC_KEY_ROTATION_THRESHOLD_ATTACKER_ADVANTAGE_MAX.
+ * Default value is 60.
+ *
+ * @param pKeyRotationThrInfo                  Reference to the key rotation threshold data
+ *
+ * @return
+ *         - \ref NVML_SUCCESS                 if \a key rotation threashold max attacker advantage has been set
+ *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
+ *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid or \a memory is NULL
+ *         - \ref NVML_ERROR_INVALID_STATE     if confidential compute GPU ready state is enabled
+ *         - \ref NVML_ERROR_NOT_SUPPORTED     if this query is not supported by the device
+ *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
+ */
+nvmlReturn_t DECLDIR nvmlSystemSetConfComputeKeyRotationThresholdInfo(
+                          nvmlConfComputeSetKeyRotationThresholdInfo_t *pKeyRotationThrInfo);
+
+/**
  * Get Conf Computing System Settings.
  *
  * %HOPPER_OR_NEWER%
  * Supported on Linux, Windows TCC.
  *
  * @param settings                                     System CC settings
  *
@@ -6271,14 +6405,15 @@
  * @param device                               Device handle
  * @param isEnabled                            Pointer to specify if GSP firmware is enabled
  * @param defaultMode                          Pointer to specify if GSP firmware is supported by default on \a device
  *
  * @return
  *         - \ref NVML_SUCCESS                 if GSP firmware mode is sucessfully retrieved
  *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid or any of \a isEnabled or \a defaultMode is NULL
+ *         - \ref NVML_ERROR_NOT_SUPPORTED     if GSP firmware is not enabled for GPU
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlDeviceGetGspFirmwareMode(nvmlDevice_t device, unsigned int *isEnabled, unsigned int *defaultMode);
 
 /**
  * @}
  */
@@ -7306,14 +7441,17 @@
  *                                              or if the fan index doesn't reference an actual fan.
  *        NVML_ERROR_NOT_SUPPORTED       if the device is older than Maxwell.
  *        NVML_ERROR_UNKNOWN             if there was an unexpected error.
  */
 nvmlReturn_t DECLDIR nvmlDeviceSetFanSpeed_v2(nvmlDevice_t device, unsigned int fan, unsigned int speed);
 
 /**
+ * Deprecated: Will be deprecated in a future release. Use \ref nvmlDeviceSetClockOffsets instead. It works
+ *             on Maxwell onwards GPU architectures.
+ *
  * Set the GPCCLK VF offset value
  * @param[in]   device                         The identifier of the target device
  * @param[in]   offset                         The GPCCLK VF offset value to set
  *
  * @return
  *         - \ref NVML_SUCCESS                 if \a offset has been set
  *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
@@ -7321,14 +7459,17 @@
  *         - \ref NVML_ERROR_NOT_SUPPORTED     if the device does not support this feature
  *         - \ref NVML_ERROR_GPU_IS_LOST       if the target GPU has fallen off the bus or is otherwise inaccessible
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlDeviceSetGpcClkVfOffset(nvmlDevice_t device, int offset);
 
 /**
+ * Deprecated: Will be deprecated in a future release. Use \ref nvmlDeviceSetClockOffsets instead. It works
+ *             on Maxwell onwards GPU architectures.
+ *
  * Set the MemClk (Memory Clock) VF offset value. It requires elevated privileges.
  * @param[in]   device                         The identifier of the target device
  * @param[in]   offset                         The MemClk VF offset value to set
  *
  * @return
  *         - \ref NVML_SUCCESS                 if \a offset has been set
  *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
@@ -7336,72 +7477,14 @@
  *         - \ref NVML_ERROR_NOT_SUPPORTED     if the device does not support this feature
  *         - \ref NVML_ERROR_GPU_IS_LOST       if the target GPU has fallen off the bus or is otherwise inaccessible
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlDeviceSetMemClkVfOffset(nvmlDevice_t device, int offset);
 
 /**
- * Set Conf Computing Unprotected Memory Size.
- *
- * For Ampere &tm; or newer fully supported devices.
- * Supported on Linux, Windows TCC.
- *
- * @param device                               Device Handle
- * @param sizeKiB                              Unprotected Memory size to be set in KiB
- *
- * @return
- *         - \ref NVML_SUCCESS                 if \a sizeKiB successfully set
- *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
- *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid
- *         - \ref NVML_ERROR_NOT_SUPPORTED     if this query is not supported by the device
- */
-nvmlReturn_t DECLDIR nvmlDeviceSetConfComputeUnprotectedMemSize(nvmlDevice_t device, unsigned long long sizeKiB);
-
-/**
- * Set Conf Computing GPUs ready state.
- *
- * For Ampere &tm; or newer fully supported devices.
- * Supported on Linux, Windows TCC.
- *
- * @param isAcceptingWork                      GPU accepting new work, NVML_CC_ACCEPTING_CLIENT_REQUESTS_TRUE or
- *                                             NVML_CC_ACCEPTING_CLIENT_REQUESTS_FALSE
- *
- * return
- *         - \ref NVML_SUCCESS                 if \a current GPUs ready state is successfully set
- *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
- *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a isAcceptingWork is invalid
- *         - \ref NVML_ERROR_NOT_SUPPORTED     if this query is not supported by the device
- */
-nvmlReturn_t DECLDIR nvmlSystemSetConfComputeGpusReadyState(unsigned int isAcceptingWork);
-
-/**
- * Set Conf Computing key rotation threshold. 
- *
- * %HOPPER_OR_NEWER%
- * Supported on Linux, Windows TCC.
- *
- * This function is to set the confidential compute key rotation threshold parameters.
- * @ref pKeyRotationThrInfo->maxAttackerAdvantage should be in the range from 
- * NVML_CC_KEY_ROTATION_THRESHOLD_ATTACKER_ADVANTAGE_MIN to NVML_CC_KEY_ROTATION_THRESHOLD_ATTACKER_ADVANTAGE_MAX.
- * Default value is 60.
- *
- * @param pKeyRotationThrInfo                  Reference to the key rotation threshold data
- *
- * @return
- *         - \ref NVML_SUCCESS                 if \a key rotation threashold max attacker advantage has been set
- *         - \ref NVML_ERROR_UNINITIALIZED     if the library has not been successfully initialized
- *         - \ref NVML_ERROR_INVALID_ARGUMENT  if \a device is invalid or \a memory is NULL
- *         - \ref NVML_ERROR_INVALID_STATE     if confidential compute GPU ready state is enabled
- *         - \ref NVML_ERROR_NOT_SUPPORTED     if this query is not supported by the device
- *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
- */
-nvmlReturn_t DECLDIR nvmlSystemSetConfComputeKeyRotationThresholdInfo(
-                          nvmlConfComputeSetKeyRotationThresholdInfo_t *pKeyRotationThrInfo);
-
-/**
  * @}
  */
 
 /** @addtogroup nvmlAccountingStats
  *  @{
  */
 
@@ -10899,17 +10982,25 @@
 /** @} */ // @defgroup nvmlGpmFunctions
 /** @} */ // @defgroup GPM
 
 #define NVML_NVLINK_POWER_STATE_HIGH_SPEED    0x0
 #define NVML_NVLINK_POWER_STATE_LOW           0x1
 
 #define NVML_NVLINK_LOW_POWER_THRESHOLD_MIN   0x1
+
+/*
+ * NVML_NVLINK_LOW_POWER_THRESHOLD_MAX will be deprecated.
+ * Use the NVML Field Value NVML_FI_DEV_NVLINK_GET_POWER_THRESHOLD_MAX
+ * to get the correct Max Low Power Threshold.
+ */
 #define NVML_NVLINK_LOW_POWER_THRESHOLD_MAX   0x1FFF
 #define NVML_NVLINK_LOW_POWER_THRESHOLD_RESET 0xFFFFFFFF
 
+#define NVML_NVLINK_LOW_POWER_THRESHOLD_DEFAULT NVML_NVLINK_LOW_POWER_THRESHOLD_RESET
+
 /* Structure containing Low Power parameters */
 typedef struct nvmlNvLinkPowerThres_st
 {
     unsigned int lowPwrThreshold;           //!< Low power threshold (in units of 100us)
 } nvmlNvLinkPowerThres_t;
 
 /**
@@ -11007,14 +11098,47 @@
  *         - \ref NVML_ERROR_NOT_SUPPORTED     if the device does not support this feature
  *         - \ref NVML_ERROR_GPU_IS_LOST       if the target GPU has fallen off the bus or is otherwise inaccessible
  *         - \ref NVML_ERROR_VERSION_MISMATCH  if the version of \a nvmlEccSramErrorStatus_t is invalid
  *         - \ref NVML_ERROR_UNKNOWN           on any unexpected error
  */
 nvmlReturn_t DECLDIR nvmlDeviceGetSramEccErrorStatus(nvmlDevice_t device,
                                                      nvmlEccSramErrorStatus_t *status);
+
+#define NVML_DEV_CAP_EGM (1 << 0) // Extended GPU memory
+/**
+ * Device capabilities
+ */
+typedef struct
+{
+    unsigned int version;               //!< the API version number
+    unsigned int capMask;               //!< OUT: Bit mask of capabilities.
+} nvmlDeviceCapabilities_v1_t;
+typedef nvmlDeviceCapabilities_v1_t nvmlDeviceCapabilities_t;
+#define nvmlDeviceCapabilities_v1 NVML_STRUCT_VERSION(DeviceCapabilities, 1)
+ 
+/**
+ * Get device capabilities
+ *
+ * See \ref  nvmlDeviceCapabilities_v1_t for more information on the struct.
+ *
+ * @param device                               The identifier of the target device
+ * @param caps                                 Returns GPU's capabilities
+ *
+ * @return
+ *         - \ref NVML_SUCCESS                         if the query is success 
+ *         - \ref NVML_ERROR_UNINITIALIZED             if the library has not been successfully initialized
+ *         - \ref NVML_ERROR_INVALID_ARGUMENT          if \a device is invalid or \a counters is NULL
+ *         - \ref NVML_ERROR_NOT_SUPPORTED             if the device does not support this feature
+ *         - \ref NVML_ERROR_GPU_IS_LOST               if the target GPU has fallen off the bus or is otherwise inaccessible
+ *         - \ref NVML_ERROR_ARGUMENT_VERSION_MISMATCH if the provided version is invalid/unsupported
+ *         - \ref NVML_ERROR_UNKNOWN                   on any unexpected error
+ */
+nvmlReturn_t DECLDIR nvmlDeviceGetCapabilities(nvmlDevice_t device,
+                                               nvmlDeviceCapabilities_t *caps);
+
 /**
  * NVML API versioning support
  */
 
 #ifdef NVML_NO_UNVERSIONED_FUNC_DEFS
 nvmlReturn_t DECLDIR nvmlInit(void);
 nvmlReturn_t DECLDIR nvmlDeviceGetCount(unsigned int *deviceCount);
@@ -11034,14 +11158,15 @@
 nvmlReturn_t DECLDIR nvmlDeviceGetComputeRunningProcesses_v2(nvmlDevice_t device, unsigned int *infoCount, nvmlProcessInfo_v2_t *infos);
 nvmlReturn_t DECLDIR nvmlDeviceGetGraphicsRunningProcesses(nvmlDevice_t device, unsigned int *infoCount, nvmlProcessInfo_v1_t *infos);
 nvmlReturn_t DECLDIR nvmlDeviceGetGraphicsRunningProcesses_v2(nvmlDevice_t device, unsigned int *infoCount, nvmlProcessInfo_v2_t *infos);
 nvmlReturn_t DECLDIR nvmlDeviceGetMPSComputeRunningProcesses(nvmlDevice_t device, unsigned int *infoCount, nvmlProcessInfo_v1_t *infos);
 nvmlReturn_t DECLDIR nvmlDeviceGetMPSComputeRunningProcesses_v2(nvmlDevice_t device, unsigned int *infoCount, nvmlProcessInfo_v2_t *infos);
 nvmlReturn_t DECLDIR nvmlDeviceGetGpuInstancePossiblePlacements(nvmlDevice_t device, unsigned int profileId, nvmlGpuInstancePlacement_t *placements, unsigned int *count);
 nvmlReturn_t DECLDIR nvmlVgpuInstanceGetLicenseInfo(nvmlVgpuInstance_t vgpuInstance, nvmlVgpuLicenseInfo_t *licenseInfo);
+nvmlReturn_t DECLDIR nvmlDeviceGetDriverModel(nvmlDevice_t device, nvmlDriverModel_t *current, nvmlDriverModel_t *pending);
 #endif // #ifdef NVML_NO_UNVERSIONED_FUNC_DEFS
 
 #if defined(NVML_NO_UNVERSIONED_FUNC_DEFS)
 // We don't define APIs to run new versions if this guard is present so there is
 // no need to undef
 #elif defined(__NVML_API_VERSION_INTERNAL)
 #undef nvmlDeviceGetGraphicsRunningProcesses
@@ -11059,14 +11184,15 @@
 #undef nvmlDeviceGetHandleByPciBusId
 #undef nvmlInit
 #undef nvmlBlacklistDeviceInfo_t
 #undef nvmlGetBlacklistDeviceCount
 #undef nvmlGetBlacklistDeviceInfoByIndex
 #undef nvmlDeviceGetGpuInstancePossiblePlacements
 #undef nvmlVgpuInstanceGetLicenseInfo
+#undef nvmlDeviceGetDriverModel
 #undef nvmlDeviceSetPowerManagementLimit
 
 #endif
 
 #ifdef __cplusplus
 }
 #endif
```

## Comparing `nvidia_nvml_dev_cu12-12.4.99.dist-info/License.txt` & `nvidia_nvml_dev_cu12-12.5.39.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_nvml_dev_cu12-12.4.99.dist-info/METADATA` & `nvidia_nvml_dev_cu12-12.5.39.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nvidia-nvml-dev-cu12
-Version: 12.4.99
+Version: 12.5.39
 Summary: NVML native dev links, headers
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
-Author-email: cuda_installer@nvidia.com
+Author-email: compute_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
```

