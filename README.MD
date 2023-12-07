Contents
Python Program:

The Python script in this branch is designed to create data in JSON format and generate a new file every minute. The code consists of the following functionalities:

The script utilizes the json, random, time, os, pytz, and datetime modules to achieve its functionalities.

Development Progress:

The script initiates a continuous loop to create a new JSON file with data points every minute. It utilizes the IST (Indian Standard Time) timezone for timestamp generation. Key functionalities include:

Creation of a new file with a timestamp.
Appending data to the JSON file.

The script is designed to run indefinitely, ensuring the regular generation of data files.

Contents
Shell Script:

The Shell script in this branch is designed to transfer files between locations. The code consists of the following functionalities:

The script utilizes the date command to retrieve the timestamp of the previous minute, constructs the file name, and then moves the file from the source to the destination.

Development Progress:

The script serves a crucial role in the overall project by ensuring the backup of data files. Key functionalities include:

Retrieving the timestamp of the previous minute.
Constructing the file name based on the timestamp.
Transferring the file from the source to the destination.

The script is designed to be executed periodically, ensuring regular backups of data files.


The development part if finished by now . The code is ready to for testing.

We executed the python program and created a cron job in which we are executing the shell script after every minute.

Commands used:

python3 create_data.py

chmod 700 create_backup.sh

how to create a cron job:

crontab -e

"A file will be open in that file add the following content in it."
* * * * * /path/of/shell/script.sh/
