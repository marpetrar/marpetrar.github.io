<div style="text-align: center;">
<p style="font-size: 20pt;">Cap Vs. Com</p>
<p style="font-size: 15pt;">A Fan's Attempt at Capcom Vs. Capcom</p>
</div>

<b><i>Developed With: C++ with SFML</i></b><br/>
<b><i>Development Time: July 2016 to December 2016</i></b>

This is my most recent project and last fan game I developed. The project began after reading the rumor about the fabled Capcom Vs. Capcom game that, had it been made, would have been based on Marvel Vs Capcom 3. I have always wanted to create a fighting game and with the lack of a Capcom Versus game, I decided to take a shot at developing a Capcom Vs. Capcom. However, with the recent announcement of Marvel Vs Capcom Infinite and ports of Ultimate Marvel Vs Capcom 3, I have decided to stop development on this fan game.

<div style="text-align: center;">
<p style="font-size: 15pt;">Framework Design</p>
</div>

Like my 2D Platform Fighter framework, I used a State Machine as the backbone with each scene representing a state. This allows for self contained sections of the game that can be easily switched between. For data that must be used by multiple states (such as the selected characters), I use an overarching class that stores the cross scene data and can be called by any state at any time.

The framework allows for varied customization of game settings such as Resolution and Controls (although said options are not available in the current demo).

Polymorphism and Inheritance is the main driving force in the class design. All characters (Playable and Assist-only) are all based off of one Fighter class with each character having a their own class that handles all unique data and mechanics. Stages work in the same maner; there is one main Stage class that all stages are based on with each stage having its own class that handles any unique mechanics and data.

Additionally, I have implemented a form of scripting that allows me to easily create custom functionality for the characters and stages. This is used to implement all of the moves and unique actions for the characters and stages.

<div style="text-align: center;">
<p style="font-size: 15pt;">Framework Design</p>
</div>

The game and framework have the following features:

<ul>
<li>Support for two players simultaneously.</li>
<li>DInput/XInput Controller support and Keyboard support</li>
<li>Dynamic detection of controllers (Only at startup in current build)</li>
<li>Marvel vs. Capcom-like Partner System</li>
<li>Support for a number of different fighting game style inputs.</li>
<li>Marvel vs. Capcom-like combo system</li>
</ul>

<div style="text-align: center;">
<p style="font-size: 15pt;">The Demo</p>
</div>

The demo has two modes, Local Vs mode, where you can fight against your friends and Training mode, where you can practice moves and combos. There are 2 playable characters (Ryu and Kyosuke) and 2 non-playable assist characters (Saki and Ton Pooh). Selecting a non-playable assist will give your main playable character double health.

The gamplay is reminiscent of Marvel vs Capcom 3. There are Light, Medium, Heavy, and Special buttons and to combo you must press each button in ascending order (L to M to H to Sp). Any move can be canceled into Special Moves such as Hadouken or into a Hyper Move such as the Shin Shoryuken.

Assists can be summoned to provide a helpful boost in battle. Be it to attack from afar or to help extend your combo, simply press the Assist button and your partner will jump on screen to help.
Assists have their share of unique moves that can be performe:

<ul>
<li>Inputting QCF + Assist will use up one special bar and perform a Snap Back which will swap out the opponent wth his Assist, if playable.</li>
<li>A Cross-Assault can be done by holding down the Assist button whcih will have your parter attack while swaping out with your current character, but this cannot be used with non-playable assists.</li>
<li>Lastly, a Hyper Swap can be done, while performing a Hyper Attack, input the motions for your assist's Hyper Attack, and your assist will swap with the current character and perform their Hyper Attack. Like the above move, this cannot be used with non-playable assists.</li>
</ul>


<b><i>This is a nonprofit prototype.</i></b><br/>
<b><i>All content used (Music, Graphics, Fonts) are owned by Capcom.</i></b><br/>
<b><i>Please support the official releases.</i></b>

<div style="text-align: center;">
<p style="font-size: 15pt;">Video:</p><br/>
<iframe width="560" height="315" src="https://www.youtube.com/embed/gS0Z03F4wWI?si=GNqjTGf5Sga7MaOh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
<br/>
<div style="text-align: center;">
<a href="http://marpetrar.github.io/">Back to Main Page</a>
</div>
