# MeloTTS API Server
A quick easy way to access [MeloTTS](https://github.com/myshell-ai/MeloTTS) through REST API calls.
## Todo
[x] Add language, speaker and speed to the api call parameters

Currently only locked to english with american accent. Easy fix if requested, or you can just change the hardcode speaker_ids before build if needed.

## Usage 
Assuming you have docker installed and setup
### Build
    git clone git@github.com:lojik-ng/MeloTTS-API-Server-Full.git
    cd MeloTTS-API-Server-Full
    docker build -t melotts-api-server-full .
 ### Run
    docker run -p 8888:8080 melotts-api-server-full
### Call API
**localhost:8888/api**

    {
        "text": "Put input here",
        "language": "EN",
        "speaker": "EN-Default",
        "speed": 1.0
    }
Response : en-us.wav

### Acknowledgement
This just a API server for the awesome work of [MeloTTS](https://github.com/myshell-ai/MeloTTS) from [MyShell](https://github.com/myshell-ai)
