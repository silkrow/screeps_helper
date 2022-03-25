# Basic Commands Used In Setting Up
---
Created on 2022/3/24, by silkrow

Edition

## Create Some Creeps

1. To create a creep with a name by the spawn called 'Spawn1',
   
        Game.spawns['Spawn1'].spawnCreep( [WORK, CARRY, MOVE], 'Harvester1' );

2. To create a creep and set its memory at the same time,

        Game.spawns['Spawn1'].spawnCreep( [WORK, CARRY, MOVE], 'Builder1', { memory: { role: 'builder' } } );

## Control the Room

1. Activate the Safe Mode,
   
        Game.spawns['Spawn1'].room.controller.activateSafeMode();

## Construction 

1. Build a StructureTower

        Game.spawns['Spawn1'].room.createConstructionSite( 23, 22, STRUCTURE_TOWER );