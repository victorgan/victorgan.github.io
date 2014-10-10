---
layout: post
title: Path Planning for Wheelchairs
---

You are on a wheelchair. You want to get across campus while avoiding all
obstacles and moving people. How does your wheelchair do this autonomously? How
does your wheelchair a) know where you want to go and confirm where it's going
and b) go there without having you to labourously avoid obstacles?

I feel real-time stategy games have a good answer. A bird's eye view map of the
area on a tablet, where the user can click on the map to tell the wheelchair
where to go. If the user wants to go somewhere else, they can click elsewhere.
Setting waypoints (shift-clicking in Starcraft) could be a feature. This is good
because the user can tell the wheelchair exactly where it wants to go, and let
the wheelchair take care of avoiding obstacles, streetlights, etc.


## Game Path Planning
Some initial research on how games like starcraft implement path planning.
- [Starcraft path finding hack](http://www.codeofhonor.com/blog/the-starcraft-path-finding-hack): they
  made SCVs float to avoid having to do path planning all the time.
- [Stackoverflow on Starcraft path planning](http://gamedev.stackexchange.com/questions/62881/how-to-do-starcraft-pathfinding)
- [Programming Game AI By Example]({% post_url 2014-10-09-programming-game-ai-by-example-mat-buckland.pdf %}).


## Ideas

- Use an updating A star search with costs around predicted locations for moving
  targets as really high.

