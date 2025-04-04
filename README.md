# CBT418
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE 418 IS FROM COMBINED INSURANCE OF AMERICA, CHICAGO        *   FILE 418
//*           ILLINOIS.  THIS FILE IS IN IEBUPDTE SYSIN FORMAT      *   FILE 418
//*           AND CONTAINS THE FOLLOWING :                          *   FILE 418
//*                                                                 *   FILE 418
//*                                                                 *   FILE 418
//*           $INDEX            CHANGES A/O JANUARY  1988           *   FILE 418
//*                                                                 *   FILE 418
//*                                                                 *   FILE 418
//*         AXFXPIRE          ACF2 LOGONID EXPIRATION UTILITY       *   FILE 418
//*                           PROGRAM THAT NEW USES THE ACF2        *   FILE 418
//*                           EXTENDED ALTER REQUEST ENTRY          *   FILE 418
//*                           (ARE) CONTROL BLOCK STRUCTURE         *   FILE 418
//*                                                                 *   FILE 418
//*         ACFVIOS           ACF2 UTILITY PROGRAM THAT WILL        *   FILE 418
//*                           COPY THE ACF2 SECURITY VIOLATION      *   FILE 418
//*                           COUNTER (SEC-VIO) TO USER-DEFINED     *   FILE 418
//*                           FIELDS AND WILL SUSPEND ANY LOGONID   *   FILE 418
//*                           WITH 6 OR MORE VIOLATIONS.            *   FILE 418
//*                                                                 *   FILE 418
//*         AXFEXPDT          THIS IS A SIMULATION VERSION OF       *   FILE 418
//*                           THE ACFXPIRE PROGRAM THAT WILL        *   FILE 418
//*                           PRODUCE A REPORT OF WHAT LOGONIDS     *   FILE 418
//*                           WILL BE EXPIRED BY THE ACFXPIRE       *   FILE 418
//*                           PROGRAM.                              *   FILE 418
//*                                                                 *   FILE 418
//*         USERCFDE          THIS IS OUR ACF2 USERFDE ENTRIES      *   FILE 418
//*                           NEEDED FOR THE ACFVIOS UTILITY        *   FILE 418
//*                           PROGRAM.                              *   FILE 418
//*                                                                 *   FILE 418
//*         USERLIDE          THIS IS OUR ACF2 USER LOGONID FIELDS  *   FILE 418
//*                           NEEDED FOR THE ACFVIOS UTILITY        *   FILE 418
//*                           PROGRAM.                              *   FILE 418
//*                                                                 *   FILE 418
//*         IVP3480           SOME CHANGES TO MY 3480 CARTRIDGE     *   FILE 418
//*                           INSTALLATION VERIFICATION PROCEDURE:  *   FILE 418
//*                                                                 *   FILE 418
//*            - CHANGE THE DATA BUFFER FROM 24K TO 32K.            *   FILE 418
//*              32K IS THE HIGHEST BLOCK SIZE YOU CAN USE.         *   FILE 418
//*                                                                 *   FILE 418
//*            - ADDED EQUATE OF DCBOPTW TO DCBBIT0 AFTER USE       *   FILE 418
//*              OF DCBD MACRO DSECT TO INDICATE WRITE VALIDITY     *   FILE 418
//*              CHECK FOR 3480 DEVICES.                            *   FILE 418
//*                                                                 *   FILE 418
//*            - SET EQUATE FOR TAPE-WRITE-IMMEDIATE MODE           *   FILE 418
//*              TO DCBOPTW FROM DCBBIT0 FOR BETTER PROGRAM         *   FILE 418
//*              UNDERSTANDING.                                     *   FILE 418
//*                                                                 *   FILE 418
//*            - ADD ADDITIONAL SYNCDEV MACRO AFTER WE ARE IN       *   FILE 418
//*              TAPE-WRITE-IMMEDIATE MODE TO INQUIRE ABOUT         *   FILE 418
//*              THE NUMBER OF DATA BLOCKS.                         *   FILE 418
//*                                                                 *   FILE 418
//*            - ISSUE A RETURN CODE MESSAGE ON THE LAST CLOSE      *   FILE 418
//*              OF THIS PROGRAM.                                   *   FILE 418
//*                                                                 *   FILE 418
//*            - CORRECTED COMMENTS WHERE POSSIBLE FOR CLARITY.     *   FILE 418
//*                                                                 *   FILE 418
//*           ACFSCAN           ACF2 LOGONID EXPIRATION UTILITY     *   FILE 418
//*                             TO EXPIRE LOGONIDS NOT USED IN      *   FILE 418
//*                             31 DAYS.  THIS PROGRAM USES A       *   FILE 418
//*                             USER-DEFINED DATE-SET (LIDSETP)     *   FILE 418
//*                             FIELD IF ACC-DATE IS BLANK.         *   FILE 418
//*                                                                 *   FILE 418
//*           IGGPRE00          DF/DS DASDM PRE-PROCESSING EXIT     *   FILE 418
//*                             THAT PERFORMS AN ACF2 RESOURCE      *   FILE 418
//*                             RULE VALIDATION TO ALLOW,LOG OR     *   FILE 418
//*                             DENY ALLOCATION TO DASD VOLUMES.    *   FILE 418
//*                                                                 *   FILE 418
//*           LGNPARMS          ACF2 LOGON PARAMETER EXIT TO        *   FILE 418
//*                             PROMPT THE TSO USER FOR A PROJECT   *   FILE 418
//*                             CODE AT LOGON TIME.  THIS CODE      *   FILE 418
//*                             IS APPENDED ONTO THE FIXED          *   FILE 418
//*                             ACCOUNTING INFORMATION AND          *   FILE 418
//*                             WRITTEN TO SMF.                     *   FILE 418
//*                                                                 *   FILE 418
//*           LGNPXIT           ACF2 LOGON POST-VALIDATION EXIT     *   FILE 418
//*                             THAT WILL ALLOW USAGE OF TSO        *   FILE 418
//*                             BY ACF2 RESOURCE VALIDATIONS        *   FILE 418
//*                             OF VTAM LUNAMES.  THIS EXIT CAN     *   FILE 418
//*                             BE USED FOR TSO DIAL-UP ACCESS      *   FILE 418
//*                             PROTECTION IF YOUR DIAL-UP LUNAMES  *   FILE 418
//*                             ARE A DIFFERENT NAMING CONVENTION   *   FILE 418
//*                             FROM YOUR LOCALS.                   *   FILE 418
//*                                                                 *   FILE 418
//*           IEFUTL            THIS SMF EXIT WILL ALLOW A          *   FILE 418
//*                             DIFFERENT JOB WAIT TIME FOR TSO     *   FILE 418
//*                             USERS VERSUS BATCH JOBS.  A TABLE   *   FILE 418
//*                             IS DEFINED FOR JOB WAIT TIMES BY    *   FILE 418
//*                             THE FIRST 2 DIGITS OF THE TSO       *   FILE 418
//*                             USERID.  DEFAULT JOB WAIT TIME IS   *   FILE 418
//*                             30 MINUTES.                         *   FILE 418
//*                                                                 *   FILE 418
//*                             THIS EXIT WILL NOT CHANGE IF THE    *   FILE 418
//*                             SMFPRMXX JWT VALUE IS CHANGED.      *   FILE 418
//*                                                                 *   FILE 418
//*           MCS               UTILITY PROGRAM TO DISPLAY THE      *   FILE 418
//*                             MASTER CONSOLE (WILL RUN ON         *   FILE 418
//*                             MVS/SP OR MVS/XA. AN XA VERSION     *   FILE 418
//*                             OF THE DIDOCS COMMAND).             *   FILE 418
//*                             THIS IS THE VERSION THAT CBT        *   FILE 418
//*                             RUNS.                               *   FILE 418
//*                                                                 *   FILE 418
//*           S000160           DFP 1.0  CHECKPOINT RESTART ZAP     *   FILE 418
//*                             TO ALLOW OS CHECKPOINTS ON          *   FILE 418
//*                             SHARED DASD                         *   FILE 418
//*                                                                 *   FILE 418
//*           S000180  DFP 2.1  DFP 2.1  CHECKPOINT RESTART ZAP     *   FILE 418
//*                             TO ALLOW OS CHECKPOINTS ON          *   FILE 418
//*                             SHARED DASD                         *   FILE 418
//*                                                                 *   FILE 418
//*           VLDEXIT           AN ACF2 DATASET PRE-VALIDATION      *   FILE 418
//*                             EXIT TO LIMIT ALL ALLOCATE /        *   FILE 418
//*                             SCRATCH / RENAME FUNCTIONS ON       *   FILE 418
//*                             DATASETS WITH THE MIDDLE -          *   FILE 418
//*                             INDEX NAME OF TEST TO VOLUMES       *   FILE 418
//*                             BEGINNNING WITH STM3**              *   FILE 418
//*                                                                 *   FILE 418
```
