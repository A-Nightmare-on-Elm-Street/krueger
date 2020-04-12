# Krueger

You know Freddy and how he is...

![Freddy Krueger](https://img.icons8.com/officel/48/000000/freddy-krueger.png)

## Motives

...

## Prerequisites

* Glasgow Haskell Compiler (GHC) 8.8.3
* Cabal 3.2
* macOS or Ubuntu 18.04 LTS

## Build

```bash
cabal update && cabal build krueger.cabal -v
```

## Invoke

### macOS

```bash
krueger/dist-newstyle/build/x86_64-osx/ghc-8.8.3/krueger-0.19.1.1/x/krueger/build/krueger/krueger repl

---- Elm 0.19.1 ----------------------------------------------------------------
Say :help for help and :exit to exit! More at <https://elm-lang.org/0.19.1/repl>
--------------------------------------------------------------------------------
```

### Linux (Ubuntu 18.04 LTS)

```bash
krueger/dist-newstyle/build/x86_64-linux/ghc-8.8.3/krueger-0.19.1.1/x/krueger/build/krueger/krueger repl

---- Elm 0.19.1 ----------------------------------------------------------------
Say :help for help and :exit to exit! More at <https://elm-lang.org/0.19.1/repl>
--------------------------------------------------------------------------------
```

## Install

### macOS

```bash
brew install ghc cabal-install
```

### Linux (Ubuntu 18.04 LTS)

```bash
sudo add-apt-repository -y ppa:hvr/ghc

sudo apt-get update

sudo apt-get install -y cabal-install-3.2 ghc-8.8.3 zlib1g-dev

echo 'export PATH=/opt/ghc/bin:/opt/cabal/bin:$PATH' >> ~/.profile

source ~/.profile
```

## Troubleshooting

### Linux (Ubuntu 18.04 LTS)

#### WSL2

* __Package repositories are unavailable__

    In WSL2 your package repositories may not be available due to a DNS resolution issue.
    
    This could be resolved by replacing the WSL2 generated IP address of the nameserver in /etc/resolv.conf to 8.8.8.8 (Google Public DNS)

## TODOs

Do we need a package?
