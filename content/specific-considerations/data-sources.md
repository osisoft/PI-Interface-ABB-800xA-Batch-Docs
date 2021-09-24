---
uid: BIF_DataSources
---

# Data sources

To enable the interface to access the Oracle server where ABB 800xA stores batch data, you must install Oracle OLEDB Provider on the interface node prior to starting the interface. Be sure to install the version of OLEDB Provider that corresponds to the version of Oracle you are running.

For each Oracle data source, you must configure the Net Service Name (set using Oracle Net Manager), Oracle database, username and password required to connect. You configure these settings using PI Event Frame Interface Manager, on the Source page.

The interface reads batch event data from the following tables in the data source.

| View/Table | Description |
|--|--|
| Task | Contains UniqueID (TaskID), BatchID, start time (UTC), end time (UTC) Procedure Path. |
| Resource_Associations | Contains Units associated with all batch recipes for Unit Procedure level (based on TaskID). |
| Task_Variables_Occurrences | Contains batch-associated data for all batches, such as Variable Name, Variable Value, Occurrence Time (UTC). The name of the source column (RESULTVALUE or VARIABLEVALUE) is returned in the [DESCRIPT] placeholder. |
| PDLMSGLOG | Contains batch-associated alarm data. |


This batch interface enables you to recover batches from restored archives in the ABB 800xA data source. To enable recovery from restored archives, launch PI Event Frames Interface Manager. On the Source settings page, check Collect batches from restored archives. Note that, if you have configured multiple data sources, the interface recovers batches from restored archives in all the data sources that you configured.
