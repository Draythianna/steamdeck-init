Make sure to set the value @ to a listen port number, 2 or greater!
*please note that display 2 is used by the main steam process
*2 will make the steamdeck screen go black but will allow a vncviewer to access steam's gui in desktop mode.

To utilize service as non root user type:

systemctl --user enable vncserver@3.service --run

To use with sudo (root) type:

sudo systemctrl enable vncserver@3.service --run

*connect via vncs ports 5902 or greater either <ipaddress>:2 or <ipaddress>::5902 
or as in direct example <ipaddress>:3 <ipaddress>::5903
  
  If you want to use vncservice or server with ssh encryption, feed it the nolocalhost commandline value in settings
  or x0vncserver cmd.
