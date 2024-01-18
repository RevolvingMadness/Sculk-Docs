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
                    reload.json
                    tick.json
        namespace/
            scripts/
                load.sk
                reload.sk
                tick.sk
    pack.mcmeta
```

A key thing to note is, in Sculk datapacks, the `load` tag runs 1 time on world startup and not every time you reload the datapack. This is mainly used for registering events. The normal `load` tag is replaced by `reload` that runs every reload and on world startup.
