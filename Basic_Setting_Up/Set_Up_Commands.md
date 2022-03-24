# Basic Commands Used In Setting Up
---
Created on 2022/3/24, by Silkrow

Edition

## Create Some Creeps

1. To create a creep with a name by the spawn called 'Spawn1',
   
        Game.spawns['Spawn1'].spawnCreep( [WORK, CARRY, MOVE], 'Harvester1' );

2. To create a creep and set its memory at the same time,

        Game.spawns['Spawn1'].spawnCreep( [WORK, CARRY, MOVE], 'Builder1', { memory: { role: 'builder' } } );