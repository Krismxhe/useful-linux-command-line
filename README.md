## Useful Linux Command Line

### linux command line
Check the number of files under a specific path
```
ls -l | grep "^-" | wc -l
```

Delete a specific file type under a particular path
```
cd /target_folder
rm *.file type
```

### zip
Zip all the files under a specific folder - './example_folder/*' to output.zip
```
zip -r output.zip ./example_folder/*
```

### scp
transferring data to the server through SCP
```
scp -r I:/example/example_folder/ mengxian@13x.7x.xx.xxx:/target_folder
```

### tmux
#### Common useful command
tmux list all sessions
```
tmux ls
```

tmux new a session, named 'example'
```
tmux new-s example
```

tmux attach to the session 'example'
```
tmux attach -t example
```
### cuda
graphic card info
'''
nvidia-smi
'''
cuda version info
'''
nvcc -V
'''
#### Switch CUDA version
cuda directory
'''
ls -l /usr/local
'''
current default directory
'''
echo $PATH
'''
cuda version switch(temporal)
'''
export PATH=/usr/local/cuda-xx.x:$PATH
'''
cuda version switch
'''
vim ~/.bashrc
'''
Add the following environment variables to the bashrc: "ESC": escape from editing, and "wq": quit and save.
'''
export PATH=/usr/local/cuda-12.0/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/cuda-12.0/lib64:$LD_LIBRARY_PATH
'''
Activate the edited the bashrc.
'''
source ~/.bashrc
'''
cuda version info
'''
nvcc -V
'''
