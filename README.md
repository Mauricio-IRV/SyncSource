# SyncSource

SyncSource is a simple Bash script for one-way synchronization between two directories.
It copies new or updated files from the source to the destination and removes files in the destination that no longer exist in the source.

**Features**
- Copies new/updated files from source to the destination.
- Removes files from the destination that no longer exist in the source.
- Automatically creates missing directories.
- Handles file names with spaces safely.
- Accepts custom paths via arguments or uses default paths.

## Usage

**Default directories**

If no arguments are provided then it falls back to the default `source` and `destination` variables

**Run with default directories**

./SyncSource.sh

**Run with custom directories**

./SyncSource.sh <sourceDir> <destinationDir>

**Show help**

./SyncSource.sh -h

**Requirements**
- Unix-like environment with bash
- Standard utilities: find, cp, rm

**Note:** You can set this up to be a cron job via your machine so that it's not a manual process.