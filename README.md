# Queue-Statistics

 1. **Recuperar informações do usuário:**

    https://br.api.riotgames.com/api/lol/BR/v1.4/summoner/by-name/Qck

        {
            "qck": {
                "summonerLevel": 30,
                "profileIconId": 710,
                "revisionDate": 1496328321000,
                "id": 4351880,
                "name": "Qck"
            }
        }


 2. **Recuperar informações da partida:**

    https://br1.api.riotgames.com/observer-mode/rest/consumer/getSpectatorGameInfo/BR1/4351880
    
        {
            "status": {
                "status_code": 404,
                "message": "Data not found"
            }
        }
 3. **Recuper informações gerais de partidas ranked's do usuário:**
    
    https://br.api.riotgames.com/api/lol/BR/v2.5/league/by-summoner/4351880/entry
    
 
        {
            "4351880": [
                {
                    "tier": "GOLD",
                    "queue": "RANKED_SOLO_5x5",
                    "name": "Nunu's Oracles",
                    "entries": [
                        {
                            "isFreshBlood": false,
                            "division": "III",
                            "isVeteran": false,
                            "wins": 47,
                            "losses": 48,
                            "playerOrTeamId": "4351880",
                            "playerOrTeamName": "Qck",
                            "isInactive": false,
                            "isHotStreak": false,
                            "leaguePoints": 23
                        }
                    ]
                }
            ]
        }
        
    https://br1.api.riotgames.com/lol/match/v3/matchlists/by-account/202396549
    
 
        {
            "matches": [
                {
                    "lane": "TOP",
                    "gameId": 1099992815,
                    "champion": 114,
                    "platformId": "BR1",
                    "timestamp": 1496195642531,
                    "queue": 420,
                    "role": "SOLO",
                    "season": 8
                },
            ],
            "endIndex": 417,
            "startIndex": 0,
            "totalGames": 417
        }

    https://br1.api.riotgames.com/lol/match/v3/matches/1099992815
    
 
        {
            "participantIdentities": [
                {
                    "player": {
                        "summonerName": "Qck",
                    },
                    "participantId": 5
                },
                {
                    "player": {
                        "summonerName": "xNegs",
                    },
                    "participantId": 10
                }
            ],
            "teams": [
                {
                    "win": "Win",
                },
                {
                    "win": "Fail",
                }
            ],
        }
