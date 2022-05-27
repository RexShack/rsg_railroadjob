# RexshackGaming
- discord : https://discord.gg/s5uSk56B65
- youtube : https://www.youtube.com/channel/UCikEgGfXO-HCPxV5rYHEVbA
- github : https://github.com/RexShack
- support rexshack : https://rexshackgaming.tebex.io/package/5114907

# Framework QBCore RedM Edition
- https://github.com/qbcore-redm-framework

# Server Game Build
- https://docs.fivem.net/docs/server-manual/server-commands/#sv_enforcegamebuild-build
- add to your server.cfg : sv_enforceGameBuild 1436

# Description
- become a part of the railroad as a conductor
- start location is valentine railway station
- conductor must be on the train at all times or the driver will quit
- if drive quits then either you can drive the train yourself, delete the train or reset the train
- use /command while in the drivers seat : /deletetrain (this deletes the train you stay where it was deleted)
- use /command while in the drivers seat : /resettrain (this deletes the train and teleports your to valentine)

# Dependencies
- qbr-core -- https://github.com/qbcore-redm-framework/qbr-core
- qbr-menu -- https://github.com/qbcore-redm-framework/qbr-menu
- rsg_notify -- https://github.com/RexShack/rsg_notify

# Installation
- ensure the above dependancies are installed and started
- extract the contents of the rsg_railroadjob.zip
- add rsg_railroadjob to your resources folder
- ensure the following is in your \qbr-core\shared\jobs.lua

### Add Job
```lua
	['railroad'] = {
		label = 'Railroad',
		defaultDuty = true,
		offDutyPay = false,
		grades = {
            ['0'] = {
                name = 'Conductor',
                payment = 25
            },
        },
```

- add the following to your "server.cfg" : ensure rsg_railroadjob
- restart your server!
- to set job use commands /setjob <playerid> railroad 0


