## Useful Linux Command Line
### Check the number of files under specific path
```
ls -l | grep "^-" | wc -l
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

