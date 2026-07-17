# OutGunnedShowcase
## NOTICE:
All the things you see here is strictly privatized code. This is purely just a showcase of design ideas and explaining different concepts created by me for the improvement of the game

## How is penetration handled?
Penetration is currently being handled via the DeMarre's Formula that is $$ P_{new}=P_{ref}*\left(\frac{V_{new}}{V_{ref}}\right)^{\alpha}*\left(\frac{M_{new}}{M_{ref}}\right)^{\beta}*\left(\frac{D_{ref}}{D_{new}}\right)^{\gamma} $$. 
where:
P = Unknown penetration depth,
\(P_{ref}\) = Known penetration depth of the reference projectile,
V = Striking velocity of the unknown projectile,
\(V_{ref}\) = Striking velocity of the reference projectile,
D = Diameter (caliber) of the unknown projectile,
\(D_{ref}\) = Diameter of the reference projectile,
M = Mass of the unknown projectile,
\(M_{ref}\) = Mass of the reference projectile

This however is only for the simple ballistic calculations of standard conventional shells.

More complicated penetration and complex armor dynamics will be from a simplified Alekseevskii-Tate equation. This equation: $$ \frac12\rho_{p}\left(V-u\right)^2+Y_{p}=\frac12\rho_{t}u^2+R_{t} $$
where:
\(\rho _{p}\) is the Density of the penetrator (the "dart"),
V is the Impact velocity of the round,
u is the Penetration velocity (the rate at which the dart burrows into the armor),
\(\rho _{t}\) is the Density of the target armor,
\(Y_{p}\) is the Yield strength (material hardness) of the dart,
\(R_{t}\) is the Target resistance to penetration

## How is suspension and tank movement handled?
Using raycasts allows the game to maintain a life-like suspension resulting in bounciness and stiffness of springs. Further more engine horsepower, transmission and gear ratios are all being used. Automatic and manual gear shifting are also being used to further improve the tank's fluidity of motion.

## How is gun handling and ballisitics handled?
While this is currently in development, the rounds are currently being raycasted, and the gun handling is being quite a pain. However introducing depth allows the barrel to be pointed properly towards what the player is looking at.

## How about a roadmap (ENTIRELY SUBJECT TO CHANGE)?
Sure, the roadmap while I cannot promise anything at all, I plan on having the basics done by Christmas '26; that is tank movement and gun handling, dynamics, friction and the enviroment for a base. The goal is to get the game in a happy and fun state. Stuff i have in the tank that is driving me to make (Multiple Single player campaigns that include: Historic battles similar to the Last Tiger from Battlefield 1, The historic events of Clarance Smoyer, The events of operation barbarossa, the Korean conflict, vietnamese conflict, The fulda gap, black hawk down, Something with the gulf war, something with the modern conflict in ukraine. All are subject to change based on how easy they are to make and the rate at which I make them are also entirely up in the air. That being said, after I get some of World War 2 up and functional, and get the multiplayer aspect handled, I plan on releasing a demo on a Steam Next Fest, a few months after giving the game to the early access world.

## THE BIG QUESTION:
What is monitization going to look like:
Frankly as a gamer first, developer second; the current state of live games sucks. I plan on charging a one time, what you see is what you get for the entire game. I use this cost to justify the cost of the campaigns, but the multiplayer is completely free with the purchase of the base game, which means no dlcs, no crazy weird stuff, no FOMO and no missing out on cool stuff.
