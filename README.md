# file-management
Scripts for moving files and renaming directories

#### [collapseDirectories.py](/collapseDirectories.py)
Based on the file path entered, this script moves any file existing below the eighth level folder in a Linux directory structure (i.e. /media/bitCurator/Storage/Collection/IncomingTransfer/BatchNumber/Disc/JobName) up to the eigth level folder. The script writes a log of all files that were moved, including their old location and their new location. The log is written in the command line utility's home directory.

#### [extractFolderNames.py](/extractFolderNames.py)
Based on the file path entered, this script extracts the names of all nested folders and writes them to a CSV file.

#### [renameDirectories.py](/renameDirectories.py)
Based on the file path entered, this script renames all nested folders according to a CSV file named 'FolderNames.csv' with the columns named 'oldFolder' and 'newFolder,' provided that there is a match between the nested folders and the names in the 'oldFolder' column. The script writes a log of all folders that were renamed, including their old name and their new name. The log is written in the command line utility's home directory.

#### [samplingScript.py](/samplingScript.py)
Based on the file path entered, the script selects every 10th file of a folder (after skipping the first file) and moves it over identically named folder in a 'sampled' directory while the skipped files are moved into an identically named folder in an 'unsampled' directory. The script also writes 'sampled' and 'unsampled' logs of all files that were moved, including their old location and their new location. The logs are written in the command line utility's home directory.
