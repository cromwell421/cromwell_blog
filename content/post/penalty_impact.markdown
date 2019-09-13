---
title: Penalty Impact
author: Jay Cromwell
date: '2019-09-12'
slug: penalty_impact
categories: []
tags:
  - NFL
  - NFLScrapR
description: 'How do penalties influence the outcome of game?'
featured_image: ''
---

I've always heard "the team that commits the least amount of penalties wins the game." It makes sense, but I wanted to dig deeper. Not every penalty is created equal, so which ones truly "penalize" the team chances of winning? How much impact does having less penalties than the opponent? Let's find out.

First, let's take a look at the Win Probability Added (WPA) from penalties. This measures how much the win probability model from NFLScrapR increases or decreases after the penalty is committed. The below graph shows all game outcomes (ties omitted) by number of penalties committed and penalty WPA totals for the game. As you can see, it is very congested, but there is a slight edge to the winning team benefiting more from penalties. With that being said, the difference is minimal and indicates not much of an impact from penalties in determining game outcome. The reasoning is likely due to the limited number of penalties committed a game. A team runs around 70-85 plays in an NFL game and averages only about 6 penalties per game. From a drive level, I assume penalties have a bigger impact and would be interesting to look at, but at the game level, it does not appear to be significant.



![Win Probability Added/Lost by Penalties per Game.](/images/penalties_win_loss_wpa_num.png)



Next, I wanted to see if teams benefited from their opponent committing penalties compared to them being penalized. The below graphs show WPA from penalties committed by the team and by the opponent vs that teams season win percentage. This is very clear, it is better to commit less (impactful) penalties than have you opponent play a sloppy penalty game. On average, teams that do not increase their opponent's chances of winning by committing penalties have a better winning percentage in the season. This makes sense and goes with the traditional narrative, but why does it counter the point made above? I think this is more indicative of the saying "better teams commit less mistakes."  When you look at an individual game, penalties don't affect the outcome much by having such little WPA impact. When we aggregate this over the season, it is a little more telling. 

They also have a bit of luck in their opponent gifting them WPA with the second graph showing a positive correlation, albeit very slight. This is not near as correlated to winning percentage as team's own penalties though, showing that the better teams are more disciplined teams.

![Team's Season Win Percentage by Penalty WPA.](/images/penalty_win_perc_penalized.png)

![Team's Season Win Percentage by Opponent's Penalty WPA.](/images/penalty_win_perc_non_penalized.png)


Finally, out of curiosity, let's take a quick look at which penalties have the biggest impact. 


![Average Penalty WPA and EPA.](/images/penalty_type_wpa_epa.png)


Since penalties don't have much game impacts, certain ones do weigh more than others. Many of the big ones are after the play, and tack on 15 yards to the end of the play, making them more significant. Obviously, the timing of the penalty is highly important as well when weighing WPA. Going forward, it would be interesting to look at which teams in particular commit the worst penalties in clutch time, but for now, we can assume that if you want to be a good team, it would help to not commit impactful penalties. If you want to win a game....that's a different story.


As always, thanks NFLScrapR for the data!


