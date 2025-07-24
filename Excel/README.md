#### Archive
To use this file, you must first complete a few steps.
First of all, you have to use Microsoft Excel 2016 version or older.

## 1. Create Macro-Enabled Excel Workbook
![Marco-Enabled](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/excel_macro_enable.PNG?raw=true)

## 2. Unlock Developer Mode 
Go to Settings -> Cusiomize Ribbon and check Developer
![DevMode](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/excel_developersMode.PNG?raw=true)

## 3. Download OPC UA Client Library for Microsoft Excel
Link: https://support.industry.siemens.com/cs/document/109748892/opc-ua-client-library-for-microsoft-excel?dti=0&lc=en-PL

## 4. Download Microsoft .NET Framework 4.7.2
Link: https://dotnet.microsoft.com/en-us/download/dotnet-framework/net472

## 5. Register the library via the command line as an administrator
Open command line as an administrator and type this command:
# C:\Windows\Microsoft.NET\Framework64\v4.0.30319\RegAsm.exe C:\OPC_UA_ExcelClient\Application\Opc.Ua.ExcelClient.dll /tlb /codebase

## How it works?
![Connect_Panel](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/connect_panel.PNG?raw=true)
# 1. Type OPC Server IP and click "Pobierz endpoint'y". After this operation, all endpoints will be written.
# 2. Select one of the endpoints, type login and password if needed and click "Połącz". A message about a successful connection will appear. Button "Odłącz" will disconnect this workbook from OPC UA server endpoint.
![Archive_Panel](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/archive.PNG?raw=true)
# 3. Type NodeId values and click "Subskrybuj". From now on every change of alarm will be stored in archive.
# 4. Button "Odsubskrybuj" will end subscription. Button "Wyczyść" clears up to 100 records in archive.

# To read NodeID's use UaExpert. Link:https://www.unified-automation.com/products/development-tools/uaexpert.html
![NodeIds](https://github.com/kcha01/Data_archiving_S7-1200PLC_WebPage_OPCServer/blob/main/Screenshots/NodeIds.png?raw=true)



