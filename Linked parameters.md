# Action Linked Parameters

## Save Linked Parameters flag

This flag, in the payload response is named `saveDataBeforeRunning`.

When you create a new action without linked parameters, this flag is also on `true` but you can't turn it to `false`.

This Bug is going to trigger any corresponding listener `On record change` over that entity before executes the Action Script.

So, if you need to solve this, a workaround is to create a linked parameter without information, disable de `Save linked parameters` flag and delete (if you need) that parameter.

To avoid this, always try to use a condition to throw the listener.

[This is a similar advice from Juanma](https://github.com/espinosajuanma/slingr-docs/blob/6edb4f8beb8ada373a311957459128d46936ad29/notes/20220831142513/README.md)