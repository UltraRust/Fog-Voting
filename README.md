# Fog-Voting
Initializes voting to remove fog from the environment

```json
{
  "Fog value to start voting 0.0 - 1.0": 0.3,
  "Interval to check the current fog (seconds)": 60.0,
  "Voting duration (seconds)": 30.0
}
```

Based on sample configuration:

Every 60.0 seconds the plugins check the fog in the game. If the value is 0.3 then the voting is going to start. Every player can vote /fogyes (keep fog) or /fogno (remove fog). Voting will be one for 30.0 seconds. If fogYES votes are more than fogNO than the fog disappears. The result is not depended on all active players. Only one player can remove the fog if nobody else is for keeping. If score is tied than the fog value doesn't change

Admin can also use commands:
/setfog - to set fog value directly (0.0 - 1.0)
/checkfog - to run the fog value check instantly
