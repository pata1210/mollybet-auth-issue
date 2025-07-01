# mollybet-auth-issue
Issue authenticating to Mollybet API via BetInAsia BLACK account – Getting 404 on login
# Mollybet API Authentication Issue via BetInAsia (BLACK)

## 🔍 Context

I'm building a value betting bot in Python and trying to connect to the Mollybet API using credentials provided by BetInAsia (BLACK account). The goal is to authenticate, retrieve sports and odds data, and detect value bets.

## ⚙️ Setup

- Credentials are stored in a `.env` file:

- Authentication request is made to:
POST https://api.mollybet.com/v1/login

- Using `requests` with basic auth and headers.

## 🧪 What Happens

All login attempts return a `404 Client Error: Not Found`:
Error HTTP al obtener el token: 404 Client Error: Not Found for url: https://api.mollybet.com/v1/login

Even trying without the `betinasiablack` suffix or with variations like `pata1210` fails.

Also tried accessing:
https://api.mollybet.com/v1/sports…after a (failed) login, and received:
404 Client Error: Not Found for url: https://api.mollybet.com/v1/sports

## 🧠 Hypotheses

- The credentials provided by BetInAsia are correct, but maybe:
  - The Mollybet API access is not yet activated for my account.
  - There’s a specific subdomain or URL I should be using instead of `api.mollybet.com`.
  - Authentication for BLACK accounts is handled differently.
  - I’m missing required headers or a step in the auth process.

## 🙏 Help Wanted

I'd greatly appreciate help from anyone who has successfully used the **Mollybet API via BetInAsia (BLACK)**. Even knowing whether the URL or method is correct would help me move forward.

Thanks in advance! 🙌

