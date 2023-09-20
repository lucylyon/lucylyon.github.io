---
title:  "Groups suck (ft. Susan)"
date:   2023-03-15
---
I was very stuck on getting the right things because of how the database is set up, but we changed it! Also I added the groups to Firebase, so now we don’t have to have them in globals.  Globals is slowly shrinking. Now the database structure makes a lot more sense, and I think I was able to get a basic appState. At least I hope I did. We will find out today. We now have events, appointments, and groups in the AppState. The events are just the names of all the activities, the appointments are schedules of which group does what when, and group just have name, age, and color. I wanted to get something done so Connor could start using it instead of trying to finish everything.

I’ve been trying to connect appState.groups to things because that shouldn’t mess with Connor’s stuff too much. However, I have been running into problems. When I added groups to Firebase, I changed the colors from hexadecimal to RGBO just so it would be easier to parse them. I do not think it is causing problems. But who knows at this point. Because groups was used in multiple places, I tried to change them all at once, which was not the smartest idea. It yelled at me, so I added groups back to globals and just called it oldGroups. That way we use it for now while I figure out what is goin on. Groups are used in five files, three of them are: for (Group g in groups) { createGroup(g) }. I still do not fully understand what createGroup does, so I’m going to talk to Connor about it today. One of them is in the appointment editor, which I do not understand one bit. Back to Connor I go. 

But! I do understand it (or thought I did) on the GroupPage. It was mapping groups, but that is no longer possible since its asynchronous. It should work the same as EventList in HDX Today, but when I mirrored it, it sure didn’t work. So I’m not sure if there’s an issue with the passing stuff around within AppState/GroupPage/GroupItem, or if it’s a problem within the AppState when I get the groups from Firebase. If Connor is having the similar problems, then it’s probably the AppState. Guess we’ll find out soon. 

Also, since Wednesday’s are busy days, Susie gets to go to daycare. Yesterday was her test day, and she was MVP! (Most Valuable Pup). So now whenever I’m doin fun Disco Tray stuff, she gets to have fun and make friends! Also this is me flexing that I now know how to put a picture in a markdown file. I took me wayy to long to figure out… 

<img src="/assets/susan.JPG" width="220" height="250"  hspace="20" vspace="20">
