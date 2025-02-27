# Misc-Batch-Files
Misc Batch Files I've Created

I occasionally write Batch Files to automate things I do in my free time. I've described them here and numbered them both here and in their filename.

1. Automatic directory compression in separate archives.

Compresses all directories in the batch file's current working directory into separate archives, with one for each directory. Uses the 7-Zip application for the compression, meaning 7-Zip must be downloaded and on Window's PATH. This command uses .7z for the archive, but can also use .zip instead if "-t7z" is replaced with "-tzip" and "%%~nG.7z" is replaced with "%%~nG.zip". This command uses max compression, but can use any of the compression levels built into the 7-Zip application by replacing the 9 in "-mx=9" with the compression level you would like. WARNING: This command OVERWRITES any previous archives of the same name and extension.

2. Automatic file compression in separate archives.

Compresses all files that are NOT .bat in the batch file's current working directory and all subdirectories into separate archives, with one for each file. Uses the 7-Zip application for the compression, meaning 7-Zip must be downloaded and on Window's PATH. This command uses .7z for the archive, but can also use .zip instead if "-t7z" is replaced with "-tzip" and "%%~nf.7z" is replaced with "%%~nf.zip". This command uses max compression, but can use any of the compression levels built into the 7-Zip application by replacing the 9 in "-mx=9" with the compression level you would like. This command can only check the current working directory and not subdirectories if "for /r %%f" is replaced with "for %%f". WARNING: This command OVERWRITES any previous compressed archives of the same name and extension.
