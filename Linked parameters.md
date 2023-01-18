# Action Linked Parameters

## Save Linked Parameters flag

This flag, in the payload response is named `saveDataBeforeRunning`.

When you create a new action without linked parameters, this flag is also on `true` but you can't turn it to `false`.

This Bug is going to trigger any corresponging listener `On record change` over that entity before executes the Action Script.

So, if you need to solve this, a workaround is to create a linked parameter without information and disable de `Save linked parameters` flag.

To avoid this, always try to use a condition to throw the listener.