This is ser2net, a program for allowing network connections to serial
ports.  See the man page for information about using the program.

Note that ser2net supports RFC 2217 (remote control of serial port
parameters), but you must have a compliant client.  The only one I
know if is kermit (http://www.columbia.edu/kermit).

If you want the opposite of ser2net (you want to connect to a "local"
serial port device that is really remote) then Cyclades has provided
a tool for this at http://www.coker.com.au/cyclades.  It is capable
of connecting to ser2net using RFC2217.

Also available is [ttynvt](https://gitlab.com/lars-thrane-as/ttynvt)
which creates a full /dev/tty device using FUSE.

----

This version includes the extra option `nosig` to ignore monitoring
of modem control lines. This is essential for it to work with 
USB UART adaptors that have no control lines.
