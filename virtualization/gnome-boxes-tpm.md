# gnome-boxes-tpm

```
sudo apt install -y ovmf
swtpm_setup --create-config-files skip-if-exist

sudo apt install -y libvirt-daemon-system libvirt-clients bridge-util
sudo systemctl start libvirtd
sudo systemctl enable libvirtd
sudo usermod -aG libvirt $USER

sudo apt install -y bridge-utils virt-manager

sudo usermod -aG kvm $USER
```

Restart.

Right click your VM > Click Preferences > Edit Configuration
Under `devices` section, add :
```
    <tpm model="tpm-crb">
      <backend type="emulator" version="2.0"/>
    </tpm>
```
