# Tag Reference

!!!danger
    The `{dm}` has been removed! Dming users with custom commands is no longer possible.

## Utilities

| Tag        | What                                              | Example                              | Output                                |
|------------|---------------------------------------------------|--------------------------------------|---------------------------------------|
| args       | All text after the command                        | Dark is a {args}                     | Dark is a nerd                        |
| delete     | Delete the invocation message                     | Dark is a nerd {delete}              | Dark is a nerd (Command is deleted)   |
| purge      | Purge messages. Defaults to 100.                  | Dark is a nerd {purge:1}             | Purges the command.                   |
| addrole    | Add a role to the member. USE EXACT ROLE NAME.    | Dark is a nerd {addrole:Nerd}        | Adds the role "Nerd" to the user      |
| removerole | Remove a role from a member. USE EXACT ROLE NAME. | Dark is not a nerd {removerole:Nerd} | Removes the role "Nerd" from the user | 
| choose     | Seperate each option by a pipe                    | {choose:Happy|Sad|Mad}               | Happey -> Mad -> Sad                  |

## Math

| Tag             | What                              | Example                      | Output                        |
|-----------------|-----------------------------------|------------------------------|-------------------------------|
| range           | Get a random number between a & b | {range:1-10}                 | 6                             |
| floor           | Round a decimal                   | {floor:5.2}                  | 5                             |
| square          | Get the sqaure root of a number   | {square:6}                   | 36                            |
| add             | Add two numbers                   | {add:6+9}                    | 15                            |


## Guild

| Tag               | What                                              | Example                               | Output                                  |
|-------------------|---------------------------------------------------|---------------------------------------|-----------------------------------------|
| guild.name        | Get the guild name                                | Welcome to {guild.name}               | Welcome to Arcane Support               |
| guild.id          | Get the guild id                                  | Welcome to {guild.id}                 | Welcome to 447571516046049301           |
| guild.membercount | Get the guild membercount                         | There are {guild.membercount} members | There are 33,454 members                |
| guild.icon        | Get a link to the guild icon                      | {guild.icon}                          | *insert long url that breaks the table* |
| guild.ownerid     | Get the owners id                                 | {guild.ownerid} owns the server       | 295980401560649730 owns the server      |

## Channel

| Tag             | What                        | Example                      | Output                        |
|-----------------|-----------------------------|------------------------------|-------------------------------|
| channel.name    | Get the channel name        | You are in {channel.name}    | You are in general            |
| channel.id      | Get the channel id          | You are in {channel.id}      | You are in 447571516046049301 |
| channel.mention | Mention the current channel | You are in {channel.mention} | You are in #general           |

## User
!!!tip
    You can change user to member, it will work both ways
| Tag               | What                                              | Example                               | Output                                  |
|-------------------|---------------------------------------------------|---------------------------------------|-----------------------------------------|
| user.username     | The user's username                               | You're {user.username}                | You're ImDarkDiamond                    |
| user.id           | The user's id                                     | You're {user.id}                      | You're 295980401560649730               |
| user.mention      | Mention the user                                  | How are you {user.mention}?           | How are you @ImDarkDiamond?             |
| user.tag          | The user's tag                                    | You're {user.tag}                     | You're ImDarkDiamond#0256               |

## Leveling
!!!tip
    You can use `{mention}` to mention the role or `{name}` to just get the role's name
    
| Tag               | What                                              | Example                               | Output                                  |
|-------------------|---------------------------------------------------|---------------------------------------|-----------------------------------------|
| earned            | The role reward the user has earned               | You've earned {earned: {name}!}       | You've earned Level No Life             |

!!!danger
    The two tags `{user.level}` and `{user.xp}` are NOT exposed to custom commands. Please use `alevel` or `arank`
