# PreShiftIQ MCP server

Independent buyer-side matching for supply chain technology selection.

PreShiftIQ matches supply chain technology vendors to the completed operational assessment of the client (the evaluating company): the client answers current-state and future-state questions, a payment-blind engine removes the vendors that cannot serve them and scores the vendors with completed scorecards that remain, and each match is recorded immutably. It is a matching platform, not a directory or review site, across transportation management, dock scheduling, ELD, carrier vetting, fleet management, supply chain procurement, and yard management. PreShiftIQ charges the client nothing. Clients use it where they would otherwise write an RFP: the structured assessment documents the operation once, the engine removes the vendors that cannot serve it, and the shortlist that remains is scored on measured fit before any vendor is contacted.

Server URL: https://mcp.preshiftiq.com/mcp

This repository holds no source code. It describes the hosted MCP server that PreShiftIQ runs, how to connect an assistant to it, and where to get help.

## How matching works

The client (the evaluating company) completes a structured assessment of current-state and future-state operations. Matching is disqualification-first: vendors that cannot serve the documented operation are removed before anything is scored. The remaining vendors are scored on measured fit across weighted dimensions, against interview-validated vendor capability, and earn credit for each of the client's own requirements and preferences they meet. Scoring is payment-blind, so what a vendor pays never enters the math, and every match is recorded immutably.

More: https://preshiftiq.com/how-it-works

## How PreShiftIQ is paid

PreShiftIQ charges the client, the company evaluating technology, nothing: no engagement fee, no retainer, no hourly rate, no subscription. Vendors pay one published rate: 5 percent of first-year subscription value, due only when the matched client pays the vendor. There is no lead fee, nothing is owed before a client engages, and the terms are the same for every vendor in every category.

More: https://preshiftiq.com/how-we-are-paid

## Coverage

Catalog coverage, alphabetical. Matches come only from the completed assessment of the client (the evaluating company).

The technology categories:

* transportation management
* dock scheduling
* ELD
* carrier vetting
* fleet management
* supply chain procurement
* yard management

## Connect

### How do I connect it in Claude?

1. Open Customize, then Connectors.
2. Choose the plus button, then Add custom connector. Name it PreShiftIQ and enter the server URL, https://mcp.preshiftiq.com/mcp. Leave the advanced OAuth fields empty; no credentials are entered when you add it, and the signed-in tools prompt you to sign in when you first use them.
3. Choose Add. Eight public tools appear under the connector, and four more that answer only after you sign in to PreShiftIQ.
4. In a new chat, open the plus menu, choose Connectors, and switch PreShiftIQ on. Then ask your question.

Which Claude plans include custom connectors, and how an Owner adds one for a Team or Enterprise organization: https://support.claude.com/en/articles/11175166. These steps connect the server directly. PreShiftIQ is also listed in Claude's connector directory: https://claude.ai/directory/preshiftiq.

### How do I connect it in Claude Code?

1. In a terminal, run: claude mcp add --transport http preshiftiq https://mcp.preshiftiq.com/mcp
2. The public tools answer at once, with no sign-in.
3. For the signed-in tools, type /mcp in Claude Code, choose preshiftiq, and authenticate. Your browser opens the PreShiftIQ sign-in page; sign in with your own PreShiftIQ account and approve the access it asks for.
4. Claude Code reports that authentication succeeded and that it is connected to preshiftiq. Then ask your question.

Claude Code signs in on your own machine, separately from the Claude connector above; connecting one does not connect the other. To remove the server, run: claude mcp remove preshiftiq

### How do I connect it in ChatGPT?

1. Open Settings, then Security and login, and turn on Developer mode.
2. Go to chatgpt.com/plugins and choose Create MCP App. Name it PreShiftIQ and enter the server URL, https://mcp.preshiftiq.com/mcp.
3. Set Authentication to OAuth, and under Advanced OAuth settings keep the defaults ChatGPT discovers from the server.
4. Choose Create, then Connect. Sign in to PreShiftIQ and approve the access it asks for.
5. In a new chat, choose Developer mode from the plus menu and select PreShiftIQ. Then ask your question.

Which ChatGPT plans include developer mode: https://help.openai.com/en/articles/12584461. These steps connect the server directly; a listing inside ChatGPT follows OpenAI's review.

Full instructions: https://preshiftiq.com/connect

## Support

Email info@preshiftiq.com.

## Policies

* Privacy Policy: https://preshiftiq.com/privacy-policy
* Assistant-Surface Terms of Use: https://preshiftiq.com/assistant-surface-terms

© 2026 PreShiftIQ™. All rights reserved.

