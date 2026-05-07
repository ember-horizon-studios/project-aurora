*The purpose of a minimalist game design document is to give a concise multimedia description of every area of the game so that you can check for synergy.*

---

## What is "\[Game Title\]"?

*Start with the broadest description of the game. Reference existing games and include visual aids if it is helpful.*

Example: *Prophecy* is a top-down multiplayer simulation game, where each player represents a "prophet", followed by a growing swarm of followers. Their goal is to traverse a procedurally-generated world, converting non-believers, conquering foes, obtaining resources, and surviving for as long as possible. The game blends some elements of traditional "god games" - like *Populous* and *Black & White* - with a simplified battle-royale model similar to agar.io.

![[populous_agario_prophecy.png]]

## Design Pillars: What is Central to the Experience?

We use design pillars to focus our design choice as we move through the project. For the purpose of this project, we want our design pillars to identify the types of fun or enjoyment which are key to the user experience. You can use the [fourteen forms of fun](https://www.gamedeveloper.com/design/fourteen-forms-of-fun) to help determine pillars.

| Power                                                                                                                | Competition                                                                                                                                                                                                                                                                | Problem Solving                                                                                                                         |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Example: Satisfaction will come from the players seeing their "flock" grow larger and larger as gameplay progresses. | Example: As the game is online, and in the agar.io competitive format, players will constantly be under threat from other player's followers. They must seek out the least occupied areas of the world and compete for resources to grow their flock and be able to fight. | Some elements of resource management and selection of appropriate upgrades will give players opportunities to feel satisfyingly clever. |

## Audience and Market

Example: This game is designed to played online with other players via Steam. A single-player "casual" mode without the competitive element will also be made available.

The game will contain some irreverent humor about religion, as well as some brutal slapstick violence. It will be aimed at a teen-adult audience.

## Core Gameplay

The player maneuvers their Prophet around the game world by using WASD control, and then used point-and-click mouse commands to give orders to the followers in the "flock".

The WASD controls directly control the Prophet, and the player-Prophet followers will use AI-path finding to stay in the general vicinity of their Prophet.

Followers start out as neutral peasants who can developed into different follower types, each having different behaviors and simple AI:

- Foragers increase a good variable by automatically scavenging for berries and nuts. They can also fight with clubs.
- Farmers obtain food when near a settlement, and also expand those farmlands when nearby. They can also fight with their pitch-forks.
- Hunters obtain food from wildlife found further away from settlements. They can also fight with their bows or spears.
- Warriors attack aggressors from other Prophets' flocks.
- Priests speed up the conversation of neutral peasants into the player's flock. They also heal other members of the flock.

Other follower types can be developed at a later date, but this list is considered the minimum viable product (MVP) version for the base game.

![[divine_inspiration_tree_cult_of_the_lamb.png]]

As the player gains faith and followers, they will be able to access and improve a tech tree, similar to the Divine Inspiration tree in *Cult of the Lamb*. Here they will be able to improve the passive attributes of different follower types, and augment their skill and abilities. This provides strategic choices, making gameplay feel different each time, while also increasing the religious theme by tying these tech-tree choices into concepts like the development, over time of religious doctrine.

## Controls

WASD - make player Prophet avatar move.

LMB click in world - highlight a resource or enemy group for targeting by relevant followers.

LMB click in interface - use HUD element, e.g. Prophet power, access skill tree or resource menus, add follower type to training queue.

RMB click - get info on game element.

## Gameplay Balance & Pacing

The game is a survival "king of the kill" game, and can therefore be played indefinitely for a player who is very skilled - or who remains unchallenged by other players. Some sessions will be very short and only last a few minutes, but more skill players should be able to play for 30-45 minutes in one go, developing their religious flock to a breathtaking size.

There should be some elements which prevent players getting too far ahead. One example of this could be culling areas of the map at set times - a mechanic similar to the storm in *Fortnite* - where a section of map is obliterated by a natural disaster, taking all residents and resources with it. This would naturally mean that, one players' following got "too big" in gameplay terms, they are often going to be taken out by things like volcanoes, floods, storm etc. This would provide some natural balancing, as these elements are easy to predict - with players being warned ahead of time - but harder to avoid with a large following.

## Character Designs

The art style of the game needs to be simple and easy to read. Given that this is a "god game"in which the player characters are meant to see humans just as a tool for their own power - the human characters in the game need to small and appear somewhat insignificant.

![[age_of_empires_and_populous_characters.png]]

Above are example from *Age of Empires* and *Populous*.

The units in *Prophecy* should be small, and the visual style needs to support the following elements of the game design:

- Visually distinct enough to have "classes" (e.g. forager, farmer, hunter, warrior, priest)
- United have "team color" clothes, as this  will be a multiplayer game with lots of players.
- Human enough to care about, abstract/small enough to not care too much about.

The visual style of the game can be 2D or 3D, but needs to allow for the above gameplay considerations.

## Setting & World

The game will aim to eventually have a procedurally generated world which changes with each new game. However, the prototype and vertical slice versions of the game should aim to have one persistent world with set locations for biomes, resources etc. For speed of production, this world will simply have the layout of the real plant Earth, with the goal being to prototype using real-world landmasses, and then switch to a more procedurally-led or customized world generation later on.

## Tone & Aesthetics

The visual style and iconography of the game will be developed as the project progresses.

Initial inspiration include the rich but moody color palette of Biblical epic movies like the Charliton Heston *Ten Commandments*, and 80s dark fantasy like Conan.

Color palettes and images.

## Narrative

This is an online player-versus-player game without an explicit narrative. The game should provide memorable moments for emergent storytelling, but besides some tutorial text, we do not intend to have dialogue or characters speaking.

## Business Model

This is a premium game, which users will purchase once and then own for good. As online-only games are heavily dependent on large user-based, the game will release as follows:

1. An initial limited-features free-demo release to gain initial interest and traction.
2. A Kickstarter campaign to raise funds to develop all features and content which are beyond the scope of this initial design document.
3. A full premium release in the under-$10 category, with Kickstarter backers receiving Steam keys plus whatever in-game rewards have been arranges.

As the full version of the game will include tech-trees and some "carry over" features (for example unlockable player colors, emblems, prophet designs etc.) it will be relatively simple to craft and appealing set of Kickstarter rewards, up to and including backer-designed elements.


