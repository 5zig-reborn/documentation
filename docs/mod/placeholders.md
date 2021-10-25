# Placeholders
Chat Filter, Auto Text, and Join Auto Text support many different placeholders that are automatically evaluated by the mod.  
All placeholders have the `${placeholder}` syntax. For example, the `username` placeholder would be `${username}`.

## List

| Syntax                 | Description                                                 | Example                                      |
| ---------------------- | ----------------------------------------------------------- | -------------------------------------------- |
| `${coords}`            | The coordinates of the player in the format `X, Y, Z`       | `0, 100, 0`                                  |
| `${coordX}`            | The X coordinate of the player.                             | `0`                                          |
| `${coordY}`            | The Y coordinate of the player.                             | `100`                                        |
| `${coordZ}`            | The Z coordinate of the player.                             | `0`                                          |
|                        |                                                             |                                              |
| `${clipboard}`         | Acts as a normal paste action (++cmd+v++ / ++ctrl+v++).     | `none`                                       |
|                        |                                                             |                                              |
| `${random[<entries>]}` | Selects a random entry from the list.                       | `${random["entry 1", "entry 2", "entry 3"]}` |
|                        |                                                             |                                              |
| `${server-ip}`         | Current IP/Domain of the server the player is currently on. | `hypixel.net`                                |
| `${server-lobby}`      | Name of the server lobby.[^1]                               | `hub-1`                                      |
| `${server-port}`       | Gives the port used for the server.                         | `25565`                                      |
| `${server-gamemode}`   | Name of the current gamemode the player plays.[^1]          |                                              |
|                        |                                                             |                                              |
| `${time-min}`          | Displays the current time in the format `HH:mm`             | `09:10`                                      |
| `${time-sec}`          | Displays the current time in the format `HH:mm:ss`          | `09:10:15`                                   |
|                        |                                                             |                                              |
| `${username}`          | Shows the name of the player.                               | `SomePlayer`                                 |
| `${uuid}`              | Shows the UUID of the player.[^2]                           | `bba224a2-0bff-4913-b042-27ca3b60973f`       |
| `${uuid-stripped}`     | Shows the UUID of the player without the dashes (`-`).[^2]  | `bba224a20bff4913b04227ca3b60973f`           |

[^1]: This may only work if the mod supports the server, either natively or via a plugin.
[^2]: Available since version 3.13.1