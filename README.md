# Gnome3-Ubuntu-Android-Termux-Test
testing with late ubuntu disco 19

On Termux:
<pre>
apt-get update && apt-get upgrade -y
apt-get install wget -y
apt-get install proot -y
apt-get install git -y
cd ~
git clone https://github.com/MFDGaming/ubuntu-in-termux.git
cd ubuntu-in-termux
chmod +x ubuntu.sh
./ubuntu.sh
cp ~/ubuntu-in-termux/resolv.conf ~/ubuntu-in-termux/ubuntu-fs/etc/
./start.sh
</pre>

On Ubuntu:
<pre>
$sudo apt-get install ubuntu-desktop gnome-shell gnome-settings-daemon mutter nautilus gnome-terminal gnome-core
</pre>

Setup VNC On Ubuntu:
<pre>
$sudo apt-get install vnc4server

$sudo cp /usr/bin/vncserver /usr/bin/vncserver.bkp
$sudo vim /usr/bin/vncserver
</pre>

Find Where It Says: 
# exec /etc/X11/xinit/xinitrcnn

then type this:
    <pre>
    "# exec /etc/X11/xinit/xinitrcnn".
       "gnome-shell &n".
       "gnome-settings-daemon &n".
       "mutter &n".
       "nautilus &n".
       "gnome-terminal &n".
       </pre>
       
       Start VNC Server On Ubuntu:
      
      <pre>
       $vncserver
       </pre>
       
       Type any 6 letter password Of Your Choice:
       <pre>
       Password: Pas123
       Verify: Pas123
       </pre>
       (REMEMBER THAT YOU CAN'T SEE WHAT YOUR TYPING IN WHEN YOU TYPE YOUR PASSWORD! SO MAKE SURE ITS CORRECT!)
       
       Check If VNC Is Working On Ubuntu:
       <pre>
       $netstat -tulpn
       </pre>
       
       Connect To Gnome3 On Your Android VNC App:
       <pre>
       Host: 127.0.0.1:5901
       (IF YOUR APP HAS A PORT OPTION, REMOVE :5901 FROM HOST AND TYPE 5901 IN PORT WITHOUT : )
       
       Password: (YOUR CHOSEN 6 LETTER PASSWORD PASSWORD)
       </pre>
       
       
       PRESS CONNECT AND LETS SEE IF WHAT HAPPENDS!
       
 
    
       
