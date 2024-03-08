# Creating a Sculk Datapack

Sculk datapacks are like regular datapacks with minor differences.

The folder structure looks like this

```
Datapack Name/
    data/
        sculk/
            tags/
                scripts/
                    load.json
                    tick.json
                    start.json
        namespace/
            scripts/
                load.sk
                tick.sk
                start.sk
    pack.mcmeta
```

A new kind of script tag is added: `start`. This only gets executed on world load and not every `/reload` like `load` does. This is mainly used for registering items & blocks. More information about that can be found [here](custom_content.md).