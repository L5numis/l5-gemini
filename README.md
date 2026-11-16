# L5 for Gemini CLI

Connect [Gemini CLI](https://github.com/google-gemini/gemini-cli) to your own store on
[L5](https://l5.com), the marketplace and auction house for ancient and world coins.

Once connected, Gemini can:

- list a coin for sale from its photos and a few details (ruler, date, denomination, reference, price)
- edit, reprice or end your listings
- consign a listed coin to an upcoming L5 auction
- show orders for coins you sold and mark them shipped with a tracking number
- show coins you bought on L5
- start an L5 provenance search from a coin's two photos (you read the results on l5.com, signed in)

It acts only on your own L5 account. It cannot buy, bid, make offers, check out, message other members
or read other members' coins. Every change is previewed first and made only after you say yes.

## Install

```
gemini extensions install https://github.com/L5numis/l5-gemini
```

Then start `gemini` and sign in:

```
/mcp auth l5
```

Your browser opens l5.com. Sign in and approve Gemini CLI. You can see and disconnect it any time in
**Settings > Connected apps** on l5.com.

Reading your store works for every member. Making changes (listing, editing, consigning, shipping,
provenance searches) needs write access: members who have completed a purchase or sale on L5 have it,
and everyone else can ask for it in **Settings > API keys** on l5.com.

## Try

- "What do I have for sale on L5 right now?"
- "List this coin on L5: ./front.jpg and ./back.jpg, Hadrian denarius, RIC II 123, $350"
- "Mark my last sale shipped, USPS tracking 9400 1000 0000 0000 0000 00"
- "Run an L5 provenance search on ./front.jpg and ./back.jpg"

## Help

- API and AI agents on L5: https://l5.com/ai
- Privacy policy: https://l5.com/privacy
- Terms: https://l5.com/terms
- Support: https://l5.com/contact or info@l5.com

This repository holds only the extension's settings (the server address and the sign-in client) and the
instructions Gemini reads. The L5 server itself runs at `https://mcp.l5.com/mcp`.
