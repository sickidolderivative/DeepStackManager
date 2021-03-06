# deepstack manager

Simple python script to list, register or delete faces in deepstack instance. Makes it easy to register face with multiple images by submitting all image files present in current directory.  

<pre>

$ dsm -h
usage: dsm [-h] [-H HOST] {register,delete,list} ...

Deepstack management tool.

positional arguments:
  {register,delete,list}

optional arguments:
  -h, --help            show this help message and exit
  -H HOST, --host HOST  Address of deepstack server


$ dsm register -h
usage: dsm register [-h] [-m MASK | -p PATH] name

positional arguments:
  name                  Name to register

optional arguments:
  -h, --help            show this help message and exit
  -m MASK, --mask MASK  Mask for files to include
  -p PATH, --path PATH  Path


$ dsm delete -h
usage: dsm delete [-h] name

positional arguments:
  name        Name to delete

optional arguments:
  -h, --help  show this help message and exit
