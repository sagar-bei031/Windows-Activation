# Windows-Activation

1. Open ``Command Prompt`` as ``Administrartor``.

2. Install product key.
   ```cmd
   cscript slmgr.vbs /ipk <product-key>
   ```
   e.g. **Windows Pro**:
   ```cmd
   cscript slmgr.vbs /ipk W269N-WFGWX-YVC9B-4J6C9-T83GX
   ```

   See [kms-client-activation](https://learn.microsoft.com/en-us/windows-server/get-started/kms-client-activation-keys?tabs=server2025%2Cwindows1110ltsc%2Cversion1803%2Cwindows81) for product key.

3. Set KMS Service
   ```cmd
   cscript slmgr.vbs /skms kms.lotro.cc
   ```

4. Activate Windows
   ```cmd
   cscript slmgr.vbs -ato
   ```

**Example Output**:
```cmd
Microsoft Windows [Version 10.0.26100.1742]
(c) Microsoft Corporation. All rights reserved.

C:\Windows\System32>cscript slmgr.vbs /ipk W269N-WFGWX-YVC9B-4J6C9-T83GX
Microsoft (R) Windows Script Host Version 5.812
Copyright (C) Microsoft Corporation. All rights reserved.

Installed product key W269N-WFGWX-YVC9B-4J6C9-T83GX successfully.


C:\Windows\System32>cscript slmgr.vbs /skms kms.lotro.cc
Microsoft (R) Windows Script Host Version 5.812
Copyright (C) Microsoft Corporation. All rights reserved.

Key Management Service machine name set to kms.lotro.cc successfully.


C:\Windows\System32>cscript slmgr.vbs -ato
Microsoft (R) Windows Script Host Version 5.812
Copyright (C) Microsoft Corporation. All rights reserved.

Activating Windows(R), Professional edition (2de67392-b7a7-462a-b1ca-108dd189f588) ...
Product activated successfully.


C:\Windows\System32
```