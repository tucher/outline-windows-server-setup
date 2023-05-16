# How to run Outline on Windows machine

1. Install WSL2
2. Install Docker, configure it to use WSL 2
3. Run Ubuntu in WSL.
4. `ln -s "/mnt/c/Program Files/Docker/Docker/resources/bin/docker.exe" /usr/local/bin/docker`
5. Ensure that docker works.
6. `chmod +x ./install_server.sh`
7. Create directory in windows FS at path OUTLINE_PATH and copy install_server.sh there
        
        
    SHADOWBOX_WIN_DIR="$OUTLINE_PATH/outline_persistent_dir" SHADOWBOX_DIR="$OUTLINE_PATH/outline_persistent_dir" $OUTLINE_PATH/install_server.sh --hostname="YOUR_HOSTNAME" --api-port=42424 --keys-port=8401