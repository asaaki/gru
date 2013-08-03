## Installation

First, git clone the repo:
```
git clone https://github.com/BananaLtd/gru.git
cd gru
```

After that, get dependencies and compile:
```
mix deps.get
mix compile
```
  
  

### Start on your slaves as a worker with

```
elixir --name gru --cookie gru --no-halt -pa ebin -pa deps/minion/ebin --app gru
```

### Start interactive with

```
iex --name gru --cookie gru -S mix
```

## What can Gru do for you?

Execute shell commands on all Nodes:

```
Gru.all "ls"
```
