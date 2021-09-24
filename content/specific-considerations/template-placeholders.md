---
uid: BIF_TemplatePlaceholders
---

# Template placeholders

The interface supports the following placeholders for defining template settings.

* BATCHID
* LEVELNUMBER (1 is procedure, 2 is unit procedure, etc.)
* OPERATION
* PARAMETER
* PHASE
* PROCEDURE
* PROCPATH (recipe path)
* TIME
* TYPE (type of task in ABB 800xA database: Batch_Batch, Batch_Phase, or Batch_RCP)
* UNIQUEID
* UNIT
* UNITPROCEDURE
* VALUE

Events from the TASK_VARIABLES_OCCURRENCES table contain the name of the source column (RESULTVALUE or VARIABLEVALUE) in the DESCRIPT placeholder.

The following placeholders are supported for ABB 800xA interfaces that are configured to collect PDLMSGLOG data:

* ASPECTNAME
* CAMPAIGNID
* CATEGORY
* CATEGORYNAME
* CLASS
* CONDITION
* EVENTCODE
* FROMVALUE
* LOCALE
* MESSAGE
* NODENAME
* OBJECTDESCRIPTION
* PATH
* PRIORITY
* PROCEDUREPATH
* QUALITY
* SEVERITY
* SOURCE
* SOURCENAME
* SUBCONDITION
* TOVALUE
* UNITID
* USERACCOUNT
* USERFIRSTACCOUNT
* USERFULLNAME
* USERSECONDARYACCOUNT
* XMLDATA
