# Brief Introduction of Memory
---
Created on 2022/3/24, by Silkrow

Edition

Each player has access to the **global** object Memory in which he/she may store any information in the JSON format. All the changes written in it are automatically stored using JSON.stringify and passed from tick to tick, allowing you memorize the setting, your own decisions, and temporary data.

The amount of memory available to a player is limited to *2 MB*.

To store some data, use

    Memory.someData = {...};

For your convenience, some game objects are **linked to** the global Memory object and store their own keys in it. For example, you may address the memory of an individual creep with the help of its memory property

    Game.creeps.John.memory = {...};

Actually, this property is an alias for a corresponding key in the global Memory object:

    Game.creeps.John.memory.role = 'harvester';
    console.log(Memory.creeps.John.role); // -> 'harvester'