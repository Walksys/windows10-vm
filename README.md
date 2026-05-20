


docker build -t walksysdev/windows10-vm .

docker run -it --rm
--device /dev/kvm
-p 6080:6080
-p 3389:3389
-v windows_data:/data
-v windows_iso:/iso
walksysdev/windows10-vm
