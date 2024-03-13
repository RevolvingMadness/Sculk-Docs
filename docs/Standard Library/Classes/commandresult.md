# CommandResult

Represents the result of running a command. (Returned from [MinecraftServer.runCommand()](minecraftserver.md#runcommandcommand-string-commandresult))

## result: [Integer](integer.md) | [Null](null.md) {data-toc-label='result'}

The result of the command. If the command did not succeed the value will default to [Null](null.md).

## succeeded: [Boolean](boolean.md) {data-toc-label='succeeded'}

Whether the command succeeded.

## errorMessage: [String](string.md) | [Null](null.md) {data-toc-label='errorMessage'}

The error message of the command. If the command succeeded the value will default to [Null](null.md).
