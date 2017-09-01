This application depends on

1. Libflowmanager
2. Libprotoident
3. Libtrace

All required packages have been added please download and run the instructions
specified in the README files.

After installing Libprotoident you need to setup the shared library

For the current session you can:

   export LD_LIBRARY_PATH=/lib:/usr/lib:/usr/local/lib or to make the change permanent
   you can add /usr/local/lib to /etc/ld.so.conf (or something it includes) and run ldconfig as root.
   If you're still having problems, running ldd [executable name] will show you the libraries it's trying
   to find, and which ones can't be found.

To Use an active device
./a.out -i wlan0 -s 1000

Use a pcap file
./a.out -i ./path/to/pcap/file.pcap
