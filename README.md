# docker-VM
Cursed docker wrapper to provide instantaneous VMs


## Usage

Create your first VM with `vm install [name] [address]`, giving it a name as well as a docker image address, such as `debian` to install a Debian VM.

Start with `vm start [name]`, and enjoy the near-instant boot times of this cursed setup.

The shared directory `/work` inside the VM will share with the automatically created `work` directory in your current working directory. X11 sharing works perfectly too, allowing you to run GUI applications from within your VM like it was running on your host! Note: you may need to run `xhost +local:127.0.0.1` to allow the VM to share your host's XServer.

When stopping your VM, use `vm stop [name]` if you'd like your changes to persist, and `vm kill [name]` if you don't need persistence.
