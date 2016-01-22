# Dino Dini said #

It is simple. If you hold the botton down before you touch the ball, you control it

If you press the button after you touch (or kick the ball dribbling) the ball you shoot it.

I wanted to retain the concept of "shoot the moment the ball is pressed" so it was the only way to make a difference.

With practice you can reliably control and pass or shoot on the fly.

One snag was that anyone with autofire on would find it impossible to control the ball. Another snag is that people never read manuals and there was no training mode to explain it.

Too many people were having problems understanding this aspect of the game and is the reason why I moved away from the model post KO2.

Sorry trapping is how passing works. If you can't trap you can't pass (well apart from using shoot to pass).

To pass you first trap the ball, point in the direction to pass and then release the button.

Sensible soccer had no trap ability at all... as I recall a short tap was the auto pass and the long tap a shot. But it is a long time ago now.

I can only tell you the way that the game was designed. If you can't trap the ball, you can't do passes (at least Auto passes).

To recap:

Touch ball then press button = Shoot
Press button then touch ball = Trap
Let go of button while trapped = pass in direction of stick
Let go of button while trapped with no stick direction = release from trap mode.

The most common reasons for people not being able to trap are:

  * Because they do not know about the fact that it depends on the order
  * Because they have autofire on their stick
  * Because they have a stick with a faulty button that does not make reliable contact

Since trapping relies on the game seeing that you are holding the button down, autofire stops you from ever giving this instruction because it is automatically pressing and releasing the button very fast. You will be able to shoot normally (although it could throw your timing off). But all traping is impossible and passing becomes vritually impossible apart from in the direction you are already facing.

When I discovered this problem with Auto Fire, I felt sick. I wondered about how many people had tried to play the game with autofire sticks and autofire on, and hated it. As a result I built a check into GOAL! to detect autofire sticks. I wish I had done the same in Kickoff 2.

Ah! that is the old slide tackle chestnut!

The problem is that with one button, how does the computer know what you mean? In a free ball situation the rules are different. Pressing the button makes you slide, unless the ball is in the air, in which case you do a header.

This makes collecting a loose ball a difficult thing to do. There is no easy way of collecting a loose ball and immediately trapping it. If you press the button after you touch it, you will shoot it... if you press it before you will slide. Providing you can slide and retain the ball in KO2 (forgive me my memory fails me on this point) then one way is to slide to the ball and keep the slide button held down. Then when you touch the ball and stop you will be in trap mode.

Once your player in in possession of the ball, sliding is no longer possible and so the problem no longer arrises.

How does this match people's experiences of the game?

# Kick Off was the first football game in which the ball was not glued on the players's feet. How did you come up with that? #

This came about because I am fanatical about simulation. Even though I was never an expert on football, I am very observant and good at breaking things down into their component parts. The development process started with me wanting to **simulate** football, down to the physics of it. I am a kind of a nut about simulations - it gives me a kick when I simulate anything from air friction to referee behavior to negotiations to how the ball bounces off the post. Nothing gives me more pleasure in game development. Any way, this is how I developed the game:

1. The first thing I made was the pitch. Logical really. Decided to make it full size, decided how much of the pitch you could see at any one time, what the viewing angle should be, the size the sprites and so on.

2. Next I made the ball. The ball is an entity in its own right. It behaves like a real ball in a lot of ways - it bounces with varying degrees of elasticity (bounce height), it has air and ground friction, it falls under gravity. So I could see the height I added the shadow. A ball should be a ball and always a ball. Apart from when the ball is carried, it is always a free entity. You can see where this is leading....

3. Next I made a single player. Naturally not wanting to cheat my simulation of a ball, I made the player dribble by bumping into the ball and knocking it forward. Ground friction will allow the player to catch up naturally. It is the same as what happens in real life.

4. After this came much struggling with trying to make it playable. Some people said I made it too hard to dribble. It is hard, but so is dribbling in football. The key thing to remember is that when you dribble you can't manipulate the ball if it has moved out of your reach. This is what makes football so exciting and why it is hard to score goals in the real game. If the ball sticks to the foot, then you might as well carry the ball in your hands. This is such a fundamental part of the mechanics of football I did not want to compromise it.