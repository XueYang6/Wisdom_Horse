# How to use wsl

### Initial setting
turn on `Hyper-V` and `Windows Subsystem for Linux` in `Turn Windows freatures on or off`

### Download wsl
run `wsl --install`
when get errors try run `wsl.exe --install -d Ubuntu`

### Transfer WSL location
1. export ubuntu system(maybe you have many of sub-linux system)
`wsl --export <Name> C:\Ubuntu\ubuntu.tar`
2. delete the original ubuntu system
`wsl --unregister <Name>`
3. import the ubuntu system where you have expoert
`wsl --import <Name> C:\Ubuntu C:\Ubuntu\ubuntu.tar`

### use clash in wsl2
add or revise file `.wslconfig` in `C:\Users\<your_name>\.wslconfig`
add content : 
``[wsl2]
networkingMode=mirrored
``
