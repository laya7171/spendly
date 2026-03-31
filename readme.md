to resume a session (claude -r)
to switch a session with another one (/resume)

General best practice is to buid a feature in a session(to manage the context window and manage the seperation of concern)
\*name the session when starting it eg:- login feature or etc, otherwise ai with write it based on the firs questino

in session if a milestone is reached then create commit (the frequently the better)

/btw = ask such question that are not part of conversation

/export (save the file as the conversation)

/logout (get out of claude code accoutn)

/login (start from start and login)

## Models in claude code

Opus (Most powerful , complex task, high token usage)
Sonet (Default, speed and quality balance, everyday coding)
Haiku(repetative, task , fastest)

Best approach use Opus for planning phase, and use sonnet fro the developement based on the plan of opus

/model (switch the model)

/usage (shows how much plan is used) (only paid ones)

/extra-usage (topup to use the more context or model more)

/stats (based on usage gives statistics)

/insights (gives a report on the user usage patter and give suggestion on how to use the claude code better)

/config (change the claude code configuration, eg thinking mode-reasoning)

/permissions (tools such as reading and writing can be used, bash tools, web search tools eg: library documenation, add custon tools using mcp)

/theme (change claude code theme light, dark)

/voice (speak to give prompt while holding the space btn)
