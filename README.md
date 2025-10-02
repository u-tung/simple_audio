# simple_audio
An Async-supported PyAudio wrapper

# Example
```python
player = Player("music_file")

# pause
player.pause()

# play
player.play()

# current_time
print(player.current_time)

# set to the start
player.current_time = 0

# set to the end
player.current_time = player.duration

# play and wait for done
player.play().wait_done()
# or
await player.play().await_done()

# close
player.close()
```
