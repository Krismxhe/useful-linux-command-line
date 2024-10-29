## Useful Linux Command Line

### Linux command line
Check the number of files under a specific path
```
ls -l | grep "^-" | wc -l
```

delete a specific file type under a particular path
```
find /example_path/directory -type f -name "*.filetype" -exec rm {} \
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

