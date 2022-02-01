//Set the selected settlement's Script name to AIStart
//Set the selected settlement's name (NOT THE DISPLAY) to S_AI1Town

//AIStart(1, "CHAOTIC", 2);
/*
By the above code you are enabling
AI for (1)player 1, (2)type of AI and
(3)level of difficulty
*/

AI1Town.obj.AsBuilding.Research("Ferocity");
AI1Town.obj.AsBuilding.Research("Ritual Chamber");
AI1Town.obj.AsBuilding.Research("Import horses");
AI1Town.obj.AsBuilding.Research("ReligiousFeast");
AI1Town.obj.AsBuilding.Research("TFoodTax");
AI1Town.obj.AsBuilding.Research("Altar of Jupiter");
AI1Town.obj.AsBuilding.Research("Cloud of Plague");
AI1Town.obj.AsBuilding.Research("Wrath of Jupiter");

//AI1Town.obj.AsBuilding.Research("God's Gift");

AI1Town.obj.AsBuilding.Research("MGladiator Shows");
AI1Town.obj.AsBuilding.Research("RGladiator Shows");
AI1Town.obj.AsBuilding.Research("Rome Training 1");
AI1Town.obj.AsBuilding.Research("Rome Training 2");
AI1Town.obj.AsBuilding.Research("Veteran Offence");
AI1Town.obj.AsBuilding.Research("Veteran Defence");
AI1Town.obj.AsBuilding.Research("Veteran Health");
AI1Town.obj.AsBuilding.Research("Heroes' Wisdom");
AI1Town.obj.AsBuilding.Research("Warriors' Wisdom");
AI1Town.obj.AsBuilding.Research("Warrior Tales");
AI1Town.obj.AsBuilding.Research("Liberati guild");
AI1Town.obj.AsBuilding.Research("Military Academy");
AI1Town.obj.AsBuilding.Research("Battle tactics");
AI1Town.obj.AsBuilding.Research("Nobility");
AI1Town.obj.AsBuilding.Research("Noble Offence");
AI1Town.obj.AsBuilding.Research("Standartization I");
AI1Town.obj.AsBuilding.Research("Standartization II");
AI1Town.obj.AsBuilding.Research("Flexibility");
AI1Town.obj.AsBuilding.Research("Statue of Isis, mother of Anubis");
AI1Town.obj.AsBuilding.Research("Statue of Osiris, father of Horus");
AI1Town.obj.AsBuilding.Research("Statue of Amon-Ra");
AI1Town.obj.AsBuilding.Research("Attack focus");
AI1Town.obj.AsBuilding.Research("Teuton Master");
AI1Town.obj.AsBuilding.Research("Barrack Level 1");
AI1Town.obj.AsBuilding.Research("Barrack Level 2");
AI1Town.obj.AsBuilding.Research("Barrack Level 3");
AI1Town.obj.AsBuilding.Research("Strenghten Stronghold Defences I");
AI1Town.obj.AsBuilding.Research("Strenghten Stronghold Defences II");
AI1Town.obj.AsBuilding.Research("Roman Archers");
AI1Town.obj.AsBuilding.Research("Roman Velit");
AI1Town.obj.AsBuilding.Research("Roman Principle");
AI1Town.obj.AsBuilding.Research("Roman Scout");
AI1Town.obj.AsBuilding.Research("Gaul Horseman");
AI1Town.obj.AsBuilding.Research("Roman Praetorian");
AI1Town.obj.AsBuilding.Research("Roman Full Armor");
AI1Town.obj.AsBuilding.Research("Roman Chariot Wheels");
AI1Town.obj.AsBuilding.Research("Gambler's Day");
AI1Town.obj.AsBuilding.Research("Gambler's Test");
AI1Town.obj.AsBuilding.Research("Gambler's Luck");
AI1Town.obj.AsBuilding.Research("Housing");
AI1Town.obj.AsBuilding.Research("Learning");

while(1)
{
	if(AI1Town.obj.player == 1)
	{
		if(GetSettlement("S_AI1Town").gold < 200000)
		{
			GetSettlement("S_AI1Town").SetGold(GetSettlement("S_AI1Town").gold + 5000 );
			GetSettlement("S_AI1Town").SetFood(GetSettlement("S_AI1Town").food + 5000 );
		}
		if(GetSettlement("S_AI1Town").population < GetSettlement("S_AI1Town").max_population)
			{
			GetSettlement("S_AI1Town").AddToPopulation (GetSettlement("S_AI1Town").max_population - GetSettlement("S_AI1Town").population);
			}				
	}
	Sleep(2000);
}
