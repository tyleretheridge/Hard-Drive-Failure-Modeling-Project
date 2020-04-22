# Hard-Drive-Failure-Modeling-Project
Creating a machine learning model to predict HDD failure based on BackBlaze's data reports.  

﻿## Unit 2 Build Project: Modeling mechanical hard drive failures in a data storage center environment  


Using BackBlaze’s data repository, I will create a machine learning classification model that will attempt to classify a storage device’s functionality status based on statistics logged from each drive's SMART stats.

**What constitutes a failed drive:**
In BackBlaze’s data, a hard drive is marked functional until the day before it fails. Drives that fail are marked as failed on the previous day’s log because if the drive is failed then it can’t report it’s status at the end of the daily reporting period. From BackBlaze’s Website @ What SMART Hard Disk Errors Actually Tell Us Regarding failure markers: 
        “Drives which have failed are marked as such and their data is no longer logged. Sometimes a drive will be removed from service even though it has not failed, like when we upgrade a Storage Pod by replacing 1TB drives with 4TB drives. In this case, the 1TB drive is not marked as a failure, but the SMART data will no longer be logged.”  
This reporting methodology means that a lack of entry does not mean failure. Only those flagged failure and lack of future entries in the log are failed.  

My data can be found at the bottom of the page here: [Backblaze Hard Drive Stats](https://www.backblaze.com/b2/hard-drive-test-data.html).




