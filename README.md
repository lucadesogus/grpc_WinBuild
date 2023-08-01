# grpc_WinBuild

### config x86 build
cmake .. -G "Visual Studio 17 2022" -A Win32 -DgRPC_SSL_PROVIDER=module -DgRPC_INSTALL=ON

### config x64 build
cmake .. -G "Visual Studio 17 2022" -A x64 -DgRPC_SSL_PROVIDER=module -DgRPC_INSTALL=ON


### release
cmake --build . --config Release -j 20 <br>
cmake --install . --prefix ./install_release --config Release

### debug
cmake --build . --config Debug -j 20 <br>
cmake --install . --prefix ./install_debug --config Debug
