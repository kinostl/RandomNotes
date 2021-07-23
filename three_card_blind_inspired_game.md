# Lore and Themes

- I want to be able to have a single player mush come out of this, I think. 
 + Single player mode would be like puzzle solving, where they're provided a pool of things to build their command deck and viruses out of.
- I'm thinking a possibility that this is like a sort of cyberpunk setting with auto-hacking?
 + Either that or ships with such complex systems they need to be dealt with by 

# Gameplay loop

- The game itself runs several rounds where it'll iterate through every players' commands. Player 1 Command, Player 2 Command, Player 3 Command, etc.
- Both player have 3 slots, that come filled with viruses. Viruses have "inserts". Things that modify them and commands that target them.
- The game runs every match composition. Player order, which viruses are in what slots, etc. This *should* be easy to keep pretty low
- Winning the round? Gain 3 Points.
- Draw the round? Gain 1 Point.
- Lost the round? Gain 0 Points.
- Whoever has the most points after all rounds (possible configurations), wins the game.
- Viruses act as sub-routines that can be dealt with through multiple means
 + Most commands tell two slots to interact
 + Some commands allow totally bypassing interacting with slots
 + An empty slot is pretty much a pass-through to the player

# Alternative Game Modes

- `Back Draft` Lose the round? gain 3 points. Draw the round? gain 1 point. Win the round? gain 0 points.

# Commands Ideas

- Commands can have some kind of cost.
- "Affinity" similar to Net Runner. You don't need to pay affiliated costs.
 + Should commands have special effects when targeting an affinity? How about for virus types?
- Definitely need to think of cycles. Do I want all Affinities to have the same types of cards with a splashed retheme?
- Instants can be better replicated by having them have some kind of bonus effect like "Target slot is immune to next command"?
- Maybe can do something similar to land destruction and "take another turn" where a command can dictate your next several commands by being some kind of command block.
- Command deck needs to come to some kind of specific card total cause of the fact that gameplay exchanges which command queue its pulling from.

## MtG Cards, Partially Converted to Commands. This is for me so I can just reinterprety or make notes.

- Fate Transfer **1{B/U}** [Instant](Move all boosts from target slot onto another target slot)
 + `Stealing` is probably a `rare mechanic` and either `expensive` or `has a requirement` such as only working on a specific type of ugprade.
- Kor Chant **1{W}** *All [Instant](Damage to this slot is instead dealt to another target slot)
 - Kor Dirge **1{U}** [Instant](All damage to this slot is instead dealt to another target slot)
 - Captain's Maneuver **{X}{R}{W}** [Instant](The next X damage that would be dealt to target creature, planeswalker, or player this turn is dealt to another target creature, planeswalker, or player instead.)
- Pit Fight **1{G/R}** [Instant](Target slot you control fights another target slot.)
 + This is definitely the `primary mechanic` of most commands. Making two slots `interact with one another`. It is Fighting is definitely a common one because it can empty a slot or cause the Inserts of the Viruses to interact. 
- Deadshot **3{R}** [Sorcery](Target slot deals damage equal to its power to another target slot. Your targetted slot does not deal damage the next time it would deal damage.)
 + This is definately another `primary mechanic`. Commands that use a creature's stat to fill in a blank.
 - Mutiny **{R}** [Sorcery](Target opposing slot deals damage equal to its power to another target opposing slot)
-  Legerdemain **{2}{U}{U}** [Sorcery](Exchange control of target artifact or creature and another target permanent that shares one of those types with it. (This effect lasts indefinitely.))
 + Could be fun to have something like "Swap control over viruses with the same type as the virus in target slot"
 + Stuff that exchanges these commands is probably an `uncommon mechanic` that is likely `expensive`
-  Fumble **{1}{U}** [Instant](Return target creature to its owner’s hand. Gain control of all Auras and Equipment that were attached to it, then attach them to another creature.)
 + This could do something like "Disable target slot and steal its upgrades."
 + `Disabling` is an `uncommon mechanic` that stops a Virus's stat for some amount of turns?
 + Maybe virus inserts need to have typings too? Upgrades, Barriers, etc.
 + Oh, that could be another fun detrimental effect - virus that can only accept inserts of a certain type
 + Inserts are upgrades to the viruses, or that things that modify commands targeting their slot.
 - True Polymorph **{4}{U}{U}** [Instant](Target artifact or creature becomes a copy of another target artifact or creature.)

-  Mage Duel **{2}{G}** [Sorcery](This spell costs {2} less to cast if you’ve cast another instant or sorcery spell this turn. - Target creature you control gets +1/+2 until end of turn. Then it fights target creature you don’t control. (Each deals damage equal to its power to the other.))
 + `This spell costs {2} less if` is the inspiring part here. I'm thinking commands that have additional effects if they're played after a command type.
 
-  Artificial Evolution **{U}** [Instant](Change the text of target spell or permanent by replacing all instances of one creature type with another. The new creature type can’t be Wall. (This effect lasts indefinitely.))
 + Maybe commands that modify the next command or opponent's next command could be neat?
 
# Insert Ideas
- See Fumble above
- Inserts should normally be free due to affinity mechanics, but can detract from the command queue's allotment otherwise.
- Inserts apply from top to bottom
- Absolute Law **{1}{W}** [Enchantment](All creatures have protection from red.)
 + Barrier that makes the virus immune to commands of certain affinities? Might be too powerful for the format.
-  Aether Web **{1}{G}** [Enchantment — Aura](Flash (You may cast this spell any time you could cast an instant.) - Enchant creature - Enchanted creature gets +1/+1, has reach, and can block creatures with shadow as though they didn’t have shadow. (Creatures with reach can block creatures with flying.))
 + `Enchanted creature gets +1/+1` is pretty similar to **Boosts**. Upgrades that just improve their power or toughness or whatever stat.
 + `has reach` or `has flying` it could be interesting to have multiple "paths" similar to flying?
 + `flash` can probably be replicated by having a command provide an upgrade to a slot, and then give it protection against the next command targetting it.
 -  Aether Tunnel {1}{U} [Enchantment — Aura](Enchant creature - Enchanted creature gets +1/+0 and can’t be blocked.)
 + `can't be blocked` can be an interesting upgrade that lets them ignore the barrier created by instants?
- https://scryfall.com/search?q=type%3Acurse&as=grid&order=name
 + curses enchant *players*. It could be fun to put something on a player that effects anything they cast. Would probably be a pretty rare one. Definitely could need to be the effect of a command.
 + Maybe players have a single barrier that modifies commands targeting them?
-  All That Glitters **{1}{W}** [Enchantment — Aura](Enchant creature - Enchanted creature gets +1/+1 for each artifact and/or enchantment you control.)
 + Boosts based on the board state would definitely be enjoyed. Those are incredibly variable and unpredictable. Maybe that should be an affinity type?
-  Angelic Destiny **{2}{W}{W}** [Enchantment — Aura](Enchant creature - Enchanted creature gets +4/+4, has flying and first strike, and is an Angel in addition to its other types. - When enchanted creature dies, return Angelic Destiny to its owner’s hand.)
 + Some kind of Insert that adds or changes the type of a virus could be really neat.
- Armadillo Cloak **{1}{G}{W}** [Enchantment — Aura](Enchant creature - Enchanted creature gets +2/+2 and has trample. - Whenever enchanted creature deals damage, you gain that much life.)
 + `Lifelink` is a straight up good ability that should be brought in, works how it should.
 + `Trample` can be adapted really good. Just means damage overloads to the player like normal.
- Arrest **{2}{W}** [Enchantment — Aura](Enchant creature - Enchanted creature can’t attack or block, and its activated abilities can’t be activated.)
 + `can't attack or block` | `can't activate abilities` - some way of shutting down a virus's upgrades or boosts for some number of turns is probably fun
-  Battle Mastery **{2}{W}** [Enchantment — Aura](Enchant creature - Enchanted creature has double strike. (It deals both first-strike and regular combat damage.))
 + `double strike` could be a really neat upgrade. Maybe any time its targetted to initiate, it initiates twice?

# Virus Ideas
- Should probably have something similar to Power and Toughness.
 + When a virus is out of Toughness, the slot is just plain empty. When a slot is empty and targetted, it counts as a 0/0 creature with anti-trample (anything fighting it gains trample while fighting it) (it just goes through)
- Some viruses come with upgrades that can not be changed.
