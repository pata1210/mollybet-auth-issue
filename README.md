# Mollybet API Authentication Issue via BetInAsia (BLACK)

## ⚙️ Context

I'm building a value betting bot in Python and trying to connect to the Mollybet API via BetInAsia (BLACK) in order to retrieve odds and detect value bets.

## 🛠️ Setup

- Credentials are stored in a `.env` file:

```env
MOLLYBET_USERNAME=your_username_here  
MOLLYBET_PASSWORD=your_password_here

👉 Important: Copy .env.example to .env and fill in your actual Mollybet credentials before running the code.

Authentication request is made to:
POST https://api.mollybet.com/v1/login
Using requests with basic auth and headers.

❗ What Happens
All login attempts return a 404 Client Error: Not Found:
Example:

Error HTTP al obtener el token: 404 Client Error: Not Found for url: https://api.mollybet.com/v1/login  
No se pudo obtener el token  

Even trying without the betinasiablack suffix or with variations like just pata1210
Also tried accessing:
https://api.mollybet.com/v1/sports
→ Same error: 404 Client Error: Not Found

🧪 Repro Steps
Clone the repo

Run python odds_fetcher.py

Output consistently shows 404 error when calling the login endpoint

🧩 Notes
.env is excluded via .gitignore

.env.example is provided for setup guidance

Using python-dotenv to load credentials

🙏 Request for Help
I'm using the official credentials they provided, and nothing seems to work, which makes me think my account is not properly activated for API access or I’m missing a key detail.

Any advice or confirmation from someone who’s used the Mollybet API via BetInAsia would be massively helpful.

Thanks!
