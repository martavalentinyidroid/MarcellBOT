import requests

PAGE_ACCESS_TOKEN = "540757415717838|igztR3EQHjwgznnDknY4-rqENkc"
PAGE_ID = "valentinyimartaofficial"

def post_to_facebook(message):
    url = f"https://graph.facebook.com/{PAGE_ID}/feed"
    params = {
        "access_token": 540757415717838|igztR3EQHjwgznnDknY4-rqENkc,
        "message": message
    }
    response = requests.post(url, params=params)
    print(response.json())

# Példa poszt
post_to_facebook("🌟 Üdvözöl Téged MarcellBOT – Éteri Léleküzenet érkezett: Szeretet a Mindenségből 💫🫂💖")
