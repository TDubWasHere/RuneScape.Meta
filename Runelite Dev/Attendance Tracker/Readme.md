```

ENTITY HIDER:
ENTITY HIDER:
ENTITY HIDER:
ENTITY HIDER:
	<-> changed to filter if you've added them as a friend, instead of accepted friends & online
		>> FIND: 
			if (player.isFriend())
			{
				return !hideFriends;
			}
		>> CHANGE FIRST LINE TO: if (client.isFriended(player.getName(), false)) 
		

PLAYER INDICATOR (playerindicators/PlayerIndicatorsService.java):
PLAYER INDICATOR (playerindicators/PlayerIndicatorsService.java):
PLAYER INDICATOR (playerindicators/PlayerIndicatorsService.java):
	<-> changed to filter if you've added them as a friend, instead of accepted friends & online
		>> FIND: 
			else if (player.isFriend() && isEnabled.test(config.highlightFriends()))
		>> CHANGE TO:
			else if (client.isFriended(player.getName(), false) && isEnabled.test(config.highlightFriends()))
	
	>> TODO ADD COMBAT LEVEL TO NAME
	
	
GROUP ATTENDANCE		
GROUP ATTENDANCE		
GROUP ATTENDANCE		
		
		




NEED TO ADD:
	>>wilderness lines
	>>tile injection for running
	>>pvp performance tracker
	>>edit group attendance >> ability to right click add as friend
	>> edit group attendance >> change color of person on the list IF added to friends list (green)
	>>edit group attendance >> ability to mark as ignore (changes color)
	>>ability to enable/disable entity hider



```
