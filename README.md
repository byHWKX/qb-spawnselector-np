# qb-spawnselector-np
qb-spawnselector np style freeeeeeeee 😜✌👌

*

no pixel style
![image](https://user-images.githubusercontent.com/89742984/169097582-614b7b8d-ebd6-4b59-b130-d83b02fbe249.png)

*

how to add it :

go to this line in qb-spawn/client.lua

[image](https://user-images.githubusercontent.com/89742984/169073088-935f1893-5b33-4c03-a57e-d9b5bf6fb056.png)

and replace it with this
```
RegisterNetEvent('qb-spawn:client:setupSpawns', function(cData, new, apps)
    if not new then
        SetNuiFocus(false, false)
        SendNUIMessage({
            type = "ui",
            status = false
        })
        choosingSpawn = false
            Wait(500)
            TriggerEvent('qb-spawnselector:opennui')
    elseif new then
        SendNUIMessage({
            action = "setupAppartements",
            locations = apps,
        })
    end
end)
```
https://discord.gg/rV7pZzCa32

