Data for each training example:
	• Label: who wins (1 for home team, 0 for away team)
	• Features:
		○ Team level statistics (home team first)
			§ Season wins
			§ Season games played
			§ Win % of last three seasons (three features)
			§ OPS, SLG, ERA, E of last three seasons (12 features)
		○ Player level statistics (per starting player)
			§ Batters (nine per team)
				□ Current season OBP, SLG, HR, BB, RBI, R, SO, AB
					® Only evaluate up to current game in season
				□ Career OBP, SLG, HR, BB, RBI, R, SO, AB
			§ Pitchers (starter only for simplification)
				□ Current season IP, BB, SO, BAOpp, ERA
					® Only evaluate up to current game in season
                □ Career IP, BB, SO, BAOpp, ERA