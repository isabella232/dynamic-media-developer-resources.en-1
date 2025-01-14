---
description: Contains supplementary messages associated with the main job log message (JobDetail). Includes warnings and other details associated with the currently processed asset.
solution: Experience Manager
title: JobLogDetailAux
feature: Dynamic Media Classic,SDK/API
role: Developer,Admin
exl-id: 789736c5-d74d-4970-9665-b43e316aca69
---
# JobLogDetailAux{#joblogdetailaux}

Contains supplementary messages associated with the main job log message (JobDetail). Includes warnings and other details associated with the currently processed asset.

 Syntax 

## Parameters {#section-2fc9bea56b6d4b72b80d4f04c5f9b862}

|  Name  | Type  | Description  |
|---|---|---|
|  logMessage  | `xsd:string`  | An auxiliary message.  |
|  logType  | `xsd:string`  |Log type: `IPSJobLog.gcUploadWarning` or `IPSJobLog.gcUploadError`.  |
|  dateCreated  | `xsd:dateTime`  | Auxiliary job log creation date.  |
