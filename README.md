# qb-spawnselector-np
qb-spawnselector np style freeeeeeeee 😜✌👌

*

no pixel style
![image](https://user-images.githubusercontent.com/89742984/169097582-614b7b8d-ebd6-4b59-b130-d83b02fbe249.png)

video : https://youtu.be/StJIssaWN5w

*

how to add it :

go to this line in qb-spawn/client.lua


![chrome_lzX609Q36v](https://user-images.githubusercontent.com/89742984/169099408-641de64e-2d83-465f-8c6c-508b3850d068.png)

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

