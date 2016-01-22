# Introduction #

The tactics positioned players depending on position of the ball on the pitch irrespective as to which side had the possession of the ball.

# Details #

Tactics can be designed using the Player Manager designer
The pitch is divided in 12 areas like this

<img src='http://openkickoff.googlecode.com/files/tacticregions.png' alt='tacticregions'>

During the game, depending on the ball location on the pitch, each players knows his home location.<br>
<br>
Since Final Whistle players movements depend on the ball position and whether the team is attacking or defending. Which gives more game strategy.<br>
<br>
<h1>Internal structure</h1>

Here is a detail about internal structure of player manager original .tac files<br>
Tactic data is stored as 10 x 80 bytes<br>
<br>
There are only 10 players because the goalie does his own thing.<br>
<br>
XY coordinates when were to stand on the pitch, the unit is pixels, with 0,0 at the top left corner flag.<br>
After that follows where the player should stand during corners, kick offs etc.<br>
The tactic description seems to be after the fisrt 800 bytes<br>
<br>
<pre><code>Loading tactics file: 5-3-2.tac<br>
playerIndex:1<br>
426, 12, 498, 387, 540, 747, 468, 1209, 480, 39, 618, 306, 648, 639, 642, 960, 432, 6, 726, 264, 786, 627, 780, 936, 666, 345, 660, 336, 636, 339, 624, 438, 426, 1, 432, 1020, 486, 1, 810, 1350<br>
playerIndex:2<br>
456, 6, 186, 261, 138, 639, 132, 927, 450, 27, 306, 312, 294, 609, 276, 969, 468, 12, 414, 390, 360, 753, 432, 1212, 276, 342, 276, 342, 324, 348, 258, 450, 450, 1, 102, 1350, 462, 1, 480, 1020<br>
playerIndex:3<br>
348, 78, 318, 276, 432, 660, 348, 984, 498, 24, 492, 318, 516, 579, 504, 810, 546, 60, 498, 327, 630, 582, 576, 954, 528, 339, 528, 339, 558, 288, 492, 501, 444, 42, 162, 1380, 468, 42, 750, 1380<br>
playerIndex:4<br>
486, 6, 372, 183, 438, 456, 438, 654, 486, 12, 450, 273, 462, 438, 468, 630, 492, 6, 510, 210, 486, 426, 468, 696, 480, 255, 480, 255, 474, 255, 474, 363, 474, 1, 504, 744, 438, 1, 408, 744<br>
playerIndex:5<br>
444, 6, 414, 324, 294, 570, 348, 756, 438, 6, 396, 315, 390, 579, 408, 807, 438, 6, 600, 276, 504, 648, 384, 894, 414, 339, 414, 339, 402, 291, 414, 492, 498, 1, 426, 744, 414, 1, 486, 744<br>
playerIndex:6<br>
132, 72, 594, 633, 588, 1059, 576, 1281, 576, 237, 708, 561, 684, 1104, 702, 1197, 732, 168, 786, 507, 804, 894, 774, 1215, 810, 513, 810, 513, 702, 636, 744, 684, 180, 18, 390, 1254, 732, 18, 894, 1380<br>
playerIndex:7<br>
174, 144, 234, 510, 210, 897, 252, 1212, 462, 189, 486, 471, 468, 792, 582, 1272, 744, 72, 678, 510, 702, 897, 684, 1203, 462, 660, 444, 522, 456, 627, 456, 678, 348, 228, 456, 1356, 564, 228, 456, 1356<br>
playerIndex:8<br>
354, 246, 210, 762, 228, 1110, 456, 1272, 444, 534, 462, 627, 456, 1026, 336, 1257, 516, 321, 702, 762, 684, 1110, 468, 1269, 510, 678, 486, 576, 516, 816, 486, 894, 558, 216, 492, 1386, 354, 216, 420, 1386<br>
playerIndex:9<br>
456, 621, 432, 924, 462, 1245, 468, 1332, 456, 717, 468, 891, 462, 1263, 450, 1293, 456, 621, 480, 924, 450, 1245, 456, 1332, 408, 678, 414, 576, 390, 816, 432, 888, 456, 516, 480, 1368, 456, 516, 432, 1368<br>
playerIndex:10<br>
120, 213, 138, 513, 120, 888, 132, 1209, 348, 246, 186, 558, 246, 1113, 234, 1200, 828, 162, 324, 642, 324, 1074, 366, 1296, 114, 522, 114, 522, 246, 636, 168, 693, 180, 42, 18, 1380, 732, 42, 522, 1254<br>
</code></pre>