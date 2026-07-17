# OutGunnedShowcase
## NOTICE:
All the things you see here is strictly privatized code. This is purely just a showcase of design ideas and explaining different concepts created by me for the improvement of the game

## How is penetration handled?
Penetration is currently being handled via the DeMarre's Formula that is 
$$
P_{new}=P_{ref}*\left(\frac{V_{new}}{V_{ref}}\right)^{\alpha}*\left(\frac{M_{new}}{M_{ref}}\right)^{\beta}*\left(\frac{D_{ref}}{D_{new}}\right)^{\gamma} 
$$

Where:
* **P** = Unknown penetration depth,
* **\(P_{ref}\)** = Known penetration depth of the reference projectile,
* **V** = Striking velocity of the unknown projectile,
* **\(V_{ref}\)** = Striking velocity of the reference projectile,
* **D** = Diameter (caliber) of the unknown projectile,
* **\(D_{ref}\)** = Diameter of the reference projectile,
* **M** = Mass of the unknown projectile,
* **\(M_{ref}\)** = Mass of the reference projectile

```console
Just Some Debugging
M61 is ready to fire at 618 m/s
Pzgr 39 weighs 6.8 kg
OF471 is a HE-Frag shell
M61 is loaded into the M1 breech
M61 failed to penetrate the Panther UFP at an impact angle of 55 degrees
```

This however is only for the simple ballistic calculations of standard conventional shells.

More complicated penetration and complex armor dynamics will be from a simplified Alekseevskii-Tate equation. This equation: 
$$ 
\frac12\rho_{p}\left(V-u\right)^2+Y_{p}=\frac12\rho_{t}u^2+R_{t}
$$

Where:
* **\(\rho _{p}\)** = Density of the penetrator (the "dart"),
* **V** = Impact velocity of the round,
* **u** = Penetration velocity (the rate at which the dart burrows into the armor),
* **\(\rho _{t}\)** = Density of the target armor,
* **\(Y_{p}\)** = Yield strength (material hardness) of the dart,
* **\(R_{t}\)** = Target resistance to penetration

# And overpressure/HE filler?
I have that set up such that the shell after penetration creates a sphere proportional to the TNT equivalent to cause damage to crew members and modules alike

## How is suspension and tank movement handled?
Using raycasts allows the game to maintain a life-like suspension resulting in bounciness and stiffness of springs. Further more engine horsepower, transmission and gear ratios are all being used. Automatic and manual gear shifting are also being used to further improve the tank's fluidity of motion.

## How is gun handling and ballisitics handled?
While this is currently in development, the rounds are currently being raycasted, and the gun handling is being quite a pain. However introducing depth allows the barrel to be pointed properly towards what the player is looking at.

## Development Roadmap
*Note: As a solo developer, timelines and features are fluid, but this is the trajectory I am building toward.*

**Phase 1: The Foundation (Target: Christmas 2026)**
* Finalizing core tank movement, environmental friction, and dynamic physics.
* Polishing gun handling and complex armor penetration mechanics to get the game into a highly playable, **fun** state.

**Phase 2: Historical WWII Campaigns**
* Developing narrative-driven, single-player scenarios based on real history (e.g., the events of Clarence Smoyer, Operation Barbarossa, and heavy atmospheric missions akin to BF1's *The Last Tiger*).

**Phase 3: Multiplayer & Early Access**
* Bringing the WWII multiplayer framework online.
* Releasing a playable demo for Steam Next Fest, followed shortly by a broader Early Access launch.

**Phase 4: Expanding the Timeline**
* Broadening the scope of conflicts to include the Korean and Vietnam Wars, the Fulda Gap scenario, Black Hawk Down, the Gulf War, and modern conflicts.

## Design & Monetization Philosophy
I am a gamer first and a developer second. I firmly believe that many modern live-service models compromise the player experience, so *OutGunned* is taking a different approach: **What you see is what you get, Respect the player's time and wallet**

* **One-Time Base Game:** A single upfront cost funds the development of the extensive single-player campaigns, with the multiplayer framework fully included.
* **Stop-Killing Games:** As a supporter of the movement, the ability to use Peer-to-Peer sessions will always exist, with absolutely zero plans to cut the game off. *You bought it, you keep it*
* **No Nonsense:** Just a complete game.
*    **Anti-FOMO Battle Passes:** Post-launch content is drip-fed through seasonal passes, but **they never expire.**
*    Fair Progression:** During an active season, progression is accelerated (1 match = 1 level). After the season ends, the pass remains permanently available in the archive to grind at a standard rate (2 matches =       1 level).
*    Rolling Rewards:** Completing any pass automatically grants you a free voucher to unlock any previously released pass from the archive.
*    Time-Saving Catch-Up:** There are no loot boxes, pay-to-win mechanics, or predatory RNG drops. If you have a busy schedule and simply don't have the time to grind, you have the option to purchase pass levels directly to get the cosmetics you want.
