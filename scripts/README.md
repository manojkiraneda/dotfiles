# openbmc-vscode
`vscode-config` is a blunt basic python script that would take arm yocto generated sdk env file as input & the target directory & creates the vscode config files in `.vscode` folder so that the intellisense features work out of the box for openbmc repositories.

## Inputs to the script
- sdk path - source sdk environment file
- target path - where the .vscode config should be created ex: openbmc/pldm
- cpp standard - the c++ standard that the openbmc/<project> supports
- configure command - the configure command [default : `meson build`]
- compile command - the compilation command [default : `ninja -C build`]
- cleanup command - the clean up command [default: `rm -rf build`]
