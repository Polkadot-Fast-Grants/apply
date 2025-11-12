📱Cards On Adventure🔥

https://tailsgamedev.itch.io/cards-on-adventure

🌟 Project Overview
Meet Cards On Adventure: a roguelike deckbuilder where every card is a character in your party! You can play the game for free in your browser, PC or mobile!

This game lives in the heart of its designers, being updated since 2020, without any source of publisher, investors nor crowdfunding yet, it will never be abandoned by the developers.

We plan to sell a "vip pass" as an NFT, using Polkadot infrastructure, giving to its owner access to all future additional content, for example new maps, cards and updates. It should also be easier for the player to resell the game in case he knows he is not going to be able to play it for a while.

Our team believes in bringing the nostalgia of reselling the game like people used to do in the past decades before everything went digital, and we hope our efforts would make it possible to do so for an even higher price than the client first paid, in charge of only a small fee for the transaction.

We invite you to watch the 40s video pitch in english.
https://youtube.com/shorts/y3Vz7YE9Ow4?si=OBcoeHregS8Nd0H_
If you happen to have a portuguese speaker, also watch Cardpybaras video pitch. It is a closely related project sent by us in the ongoing Game Jam Plus, and it is the most popular game currently among all 274 entries.
https://www.youtube.com/shorts/clnLuSUK6QQ

🔍 Project Details
Technology stack: Unity Game Engine, Polkadot.NET, rust
Core components of the game:
Battle: First the enemy places 4 cards in the battlefield, then it’s our turn to do the same. Put the tanks ahead, the archers and mages in the backline, and calculate the best spot for the supports. The cards have many roles and situations to add more strategy and fun to this move.
With your 4 cards in the battlefield, you can reposition them and proceed to the attack state by hitting the button in the bottom, which also can trigger some skills like “Heal” and “Bless”.
Then it’s time to attack. For that just drag and drop a card from your battlefield to the target card, in the enemy battlefield. It will do damage and possibly trigger more skills. And then you pass the turn. For every card death, the commander loses a life point, so when it reaches zero, he is defeated. It’s a very innovative, simple yet engaging loop.
Map progression: You go on a map from the very first spot to the end where the villain boss lives.
Story: character dialogs and decisions about the lore that may lead to rewards or penalties.
Inn: a place to rest, restoring commander’s life points and merging cards into stronger versions.
Guild: a place where you can buy potions and new adventure cards in exchange for some gold.

About the stack:
Unity: Used to build the game and it’s mechanics and resources;
Polkadot.NET, in the game’s source code. Allows the game to interact with the Polkadot ecosystem as it allows the client to operate within polkadot;
Rust: The smart contract that will run inside the chain. Written in rust it implements all the logic necessary to generate and manage the NFTs and is the basis of the monetization strategy of the game.

Architecture:
The project relies on MVC architecture adapted to Unity. The state machine pattern also plays a key role in the battle system. It uses scriptable objects to store config data.

Previous works:
It’s important to mention the system was rebuilt from zero in the new project Cardpybaras, so Cards On Adventure will be continued from this fresh code, that follows all best practices the team has accumulated during the past 7 years of professional experience. The new project is available to play here.

Screenshots:
https://drive.google.com/drive/folders/1QEM80kubtgS1t72-duNh7zAS2sFQs2Mw?usp=sharing

We aim to build the first map the best way we can, with all features shown in project details, as for now it’s lacking some of them, like the Guild, and later on we hope to launch many maps as we gather more investment and sell more game copies. In the future we hope to sell new maps packed together with new characters that will be available in that map. Also every map should have a ranking that resets periodically, so players can know who is the best at that adventure.

🧩 Ecosystem Fit
Cards On Adventure is clearly an entry game for NFT. It is completely soft in NFT monetization, so players can break the barriers to deal with this technology or to give it a new try, even if blockchain games had disappointed them in the past. It offers an advantage in comparison to buying games in the most common platforms, where products are not viable to resell.
In fact, the game can be sold on traditional platforms as well, and it would be beneficial for Polkadot to do so, as it would be propaganda for the ecosystem, and new players could compare and see this clear advantage when deciding if to buy the game here or there.
The target audiences for this game are roguelike deckbuilder players, who happen to like tabletop RPG as well. They are mostly male between 14 and 35 years old, but it can appeal to all genres and ages, whoever wants to have quick fun with an accessible digital card game.
Polkadot ecosystem has already heard of roguelike deckbuilders through “Full House Fury”, although it’s quite hard to find anything about the game on the web. Our project is already online so anyone can play. It’s just going to be improved and sold also in the blockchain. Our game is innovative even in the traditional market, so no doubts it would add to Polkadot as well.

👥 Team
Team Name: TailsGameDev
Contact Name: Cainã Correa Caldas
Contact Email: cainacc@hotmail.com
Website: https://tailsgamedev.itch.io/
Team members:
Cainã Correa Caldas
Thayse Fortes
Jonas de Souza Martins

LinkedIn Profiles (if available)
https://www.linkedin.com/in/tailsgamedev/
https://www.linkedin.com/in/thaysefortes/

Team Code Repos
https://github.com/TailsGameDev/CardsOnAdventure
https://github.com/TailsGameDev/Cardpybaras
(please request access)

GitHub Profile
https://github.com/TailsGameDev

Team's experience
Please describe the team's relevant experience, including any previous blockchain projects or contributions to the ecosystem.
Cainã Correa Caldas: 7+ years experienced in professional game development, Caldas has worked in the complex 3D multiplayer game Chasers Dash and Bash, and also in the widely recognized story driven game Truth and Tales, among other titles. He is also currently studying Computer Science in the Federal University of Santa Catarina, having blockchain lessons with Jean Everson Martina (https://www.linkedin.com/in/jean-everson-martina/) and also getting some blockchain guidance from Leonardo Custodio (https://www.linkedin.com/in/leogcustodio/), who presented him this fast grant program.
Thayse Fortes: Graduated in Animation from the Federal University of Santa Catarina. With experience in 2D character animation for TV and games. Generalist 2D artist.
Jonas de Souza Martins: Writer of “Desenredo” and “Guerra à Ruína” books, and also author of some indie games narrative.

📊 Development Status
https://github.com/TailsGameDev/Cardpybaras
We are participating on Game Jam Plus with the game Cardpybaras, please note it is the current most popular game in the competition, you can verify this in this link "https://itch.io/jam/gamejamplus-2526-10th-edition-/entries", as games there are explicitly sort by popularity. Cardpybaras concepts are heavily inspired in Cards On Adventure. The code is so fresh and clean we intend to bring the arts of Cards On Adventure to the new project and continue both games development there.
Now the systems follow best guidelines like the MVC pattern, scriptable objects for config storage, a robust state machine implementation for the whole game and also inside battles. We are also packing images into atlases, setting the best engine config for optimization, avoiding unnecessary inheritance from MonoBehaviour, yet also building modular and readable code.

📅 Development Roadmap

Number	Deliverable	Specification
0a. License: fully protected by standard copyright law.
0b. Documentation: We will have active social media and communities, so our players are always aware of what is happening. About our code it’s commented and it’s pretty readable on its own. AI can also explain that so it shouldn’t be hard to understand.
0c. Testing: You can test the game by playing it, take notes and leave feedback to us. We will be always improving it as this project lives in our hearts.
0d. Article: We will publish an article that explains what was done/achieved as part of the grant.

1 Integrate with the Polkadot ecosystem, so the season pass becomes an NFT and can be used, sold to clients, and among them with a small fee.
2 Bring all arts from Cards On Adventure to Capybara’s game, restarting the features from the point where Capybaras has stopped. Therefore bringing 2 backgrounds, 10 character arts, the game logo and icon.
3 Implement more visual effects and polish.
4 Implement rewards in the form of cards. The player should pick a card to add to the deck among 3 options.
5 Implement persistent commander life points, as well as resting to restore them, and card merging, in the Inn spot.
6 Implement gold rewards and the Guild spot where the player can basically buy cards among a greater variety in comparison to regular card rewards.
7 Implement difficulty progression, so the player gets harder fights on each spot until it gets to the villain’s boss.
8 Implement the game settings screen: language selection (english, portuguese or spanish), music and sfx volume, enemy speed, social media buttons and credits.
9 Implement the narrative/decision spots with character dialogs and rewards.

💰 Budget Breakdown

Milestone	Deliverables	Cost (USD)	Estimated Completion
1	Features 1, 2, 3	$5,000	1 month
2	Features 4, 5, 6	$5,000	1 month
3	Features 7, 8, 9	$5,000	1 month

For every deliverable the resources will be spent in:
$3,000 for Caldas (programmer, game designer, company owner), $1,000 for Thayse (2D artist), $1000 for Jonas (writer). Caldas working full-time (40h a week), and Thayse and Jonas working part time (20h a week).

Total Costs: $15,000

🔮 Future Plans

The team envisions the game as a way to introduce new people to the Polkadot ecosystem. As video games continue to build presence in nowadays culture, popularising more and more. We believe that the game is a great opportunity for Porkadot to enter this demographic. Gamers are more susceptible to new technologies and even with the popularity increase in NFT games a few years ago we still understand lighter, user experience oriented games can elevate the genre to new heights of popularity and Polkadot with it.

The game’s content is to be continuously expanded. New playable maps, characters and cosmetic items. As the community builds up online and in-person events will be introduced in order to build up hype for upcoming releases, increase sales of seasonal passes and warm up the marketplace.

For that it is crucial to establish partnerships with community leaders early on, such as content creators. Since they are a very effective means of communication between players and the team. It is also important to grow the community through social media. It is a very common and inexpensive strategy to give mild rewards for players that are active within the games’ social media communities.

The funding resources would be allocated mainly to the code necessary to integrate the game with the ecosystem and the next phase of the game’s development. Used to build content and bring the game’s world to life alongside the dev team and the artist that will continue to build new mechanics, characters, scenarios and stories. After all, the whole purpose of the game is to create a custom made experience for the player and introduce him to a new, fun world alongside NFTs.

ℹ️ Additional Information

Cards On Adventure was an official selection for STUN game festival, it also got among the best 5 pitches in FLIC and it’s an official presence in Passeio Geek two times, as well as in Nerd Show Fest, in Florianópolis, Brazil. We hope Capybara’s game is very likely to win some prizes at Game Jam + 2025/2026. The game trailer went live on the NoLobby show, that’s a big Brazilian podcast on gaming.
TailsGameDev instagram has past 1370 followers, and it keeps growing, as well as other social media and the Discord community. The company is associated with ASC Jogos, and the owner, Caldas, is known in the local game development scene.