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

First, let's take a look at the Win Probability Added (WPA) from penalties. This measures how much the win probability model from NFLScrapR increases or decreases after the penalty is committed. The below graph shows all game outcomes (ties omitted) by number of penalties committed and penalty WPA totals for the game. As you can see, it is very congested, but there is a slight edge to the winning team benefiting more from penalties. With that being said, the difference is minimal and indicates not much of an impact from penalties in determining game outcome. The reasoning is likely due to the limited number of penalties committed a game and the overall insignificance they have in WPA. A team runs around 70-85 plays in an NFL game and averages only about ~7 penalties per game. The most common of these penalties are not impactful (5 yards ~ offsides, false start, etc). Later we will see which penalties have the biggest impact, but from a high-level, penalties do not seem to carry much weight in deciding the outcome of a game. 



![Win Probability Added/Lost by Penalties per Game from 2009 - 2018.](/images/penalties_win_loss_wpa_num.png)


Next, I wanted to see if teams benefited from their opponent committing penalties compared to them being penalized. The below graphs show WPA from penalties committed by the team and by the opponent vs that teams season win percentage. This is clear, it is better to commit less (impactful) penalties than to have your opponent play a sloppy penalty game. But again, there is not a strong correlation between the two variables in either graph, illustrating the point made above. 


![Team's Season Win Percentage by Penalty WPA (2009 - 2018.](/images/penalty_win_perc_penalized.png)

![Team's Season Win Percentage by Opponent's Penalty WPA (2009 - 2018).](/images/penalty_win_perc_non_penalized.png)


Finally, out of curiosity, let's take a quick look at which penalties have the biggest impact. 


![Average Penalty WPA and EPA.](/images/penalty_type_wpa_epa.png)


Since penalties don't have much game impacts, certain ones do weigh more than others. Many of the big ones are after the play, and tack on 15 yards to the end of the play, making them more significant. Obviously, the timing of the penalty is highly important as well when weighing WPA. 

Going forward, it would be interesting to look at which teams in particular commit the worst penalties in clutch time, as well as how being on defense vs offense plays a part in penalty impact.


As always, thanks NFLScrapR for the data!


