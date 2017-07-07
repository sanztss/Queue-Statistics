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
    
    
