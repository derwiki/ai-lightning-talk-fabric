## Prerequisite
export YOUTUBE_API_KEY
export OPENAI_API_KEY

fabric -y 'https://www.youtube.com/watch?v=EWvNQjAaOHw' | fabric -p extract_wisdom
fabric -y 'https://www.youtube.com/watch?v=EWvNQjAaOHw' | tee transcript.txt && cat transcript.txt | fabric -u

fabric -u https://github.com/danielmiessler/fabric/ -p analyze_claims

## The Good
Feels very philosophically UNIX: providing plumbing so it can be used everywhere
Although, I still haven't figured out a way to build this into a workflow
code_helper could be neat but Cursor and other well-known projects have the momentum

## The Bad
Some of these patterns scale from silly to dangerous, for the same reasons that all prompt engineering does


## The Promise?
I like bringing this into command line pipes
I think LLM is still not fully understood in say, what it can be used for. Something like improve_prompt make a lot of sense.
I don't want to keep track of it, so I'm happy they are
- maybe different flavors of "improve"

## The Weird
I guess this prompt is worth having
https://github.com/danielmiessler/fabric/blob/main/patterns/explain_math/system.md

## Pattern Highlights
### improve_prompt

### create_mermaid_visualization
https://mermaid.live/edit#pako:eNqFU8ty2jAU_RWN1oTBL2y86EzAJKQFwiSki4ouVFuAJrbkynKmFPPvvcgG7MmiWumce3TfOuJYJgyHeKdovkfraCMQnHuykoWOqUrQnG9ZfIhThhaUp0z9RHd3X6pXJpICTTOgKjQmbwUYmqe1XVNdFugtT6hmFZpc_TWqiVFFXLFYG8do-sGELioUEXNDEdW0EUdGPAdPha51FZqSOkRHsuYZSGiWV-iBXEEn5FrR-J2L3TXeI3lhRS5FwdohH43Y1IcmUmgTc0ZqYiyTQ6ObGd2DktmlGU_khhrRkxEtefwuaAbd-Eou907PZlQkKYOuKiUVZPaNmBsyPKQM4lpelL_qcdWdWh9yVtSW80lMU7kUaD2-sVOLrBSHQi4TMKRNzFA7nEMilvIPprq0C33SpRJd1qtzbChYikuOZiAQtYPsDnI6yO0g71OtE5ll0IhmC_9X7pzcJwlqreX5LMgr34kyb1FL8p0pvuWdqp6bxi-lBlNMz95b5hWZsTRHL-x3CQv2uXQzTTRvg0UbLNvguQ1WZxe4B5-RJzjUqmQ9nDEFqwQQH8_SDdZ7lrENDuGasC0tU73BG3GCZzkVP6TMLi-VLHd7HG5pWgAqzVeMOIV23iSQNlMTWQqNQ8vyjQ8cHvEfHA76ru3YvjVyRr7nDUbDYQ8fcBj4_cB2gqE7dO2Ba42CUw__NVEHfd-3Hc_yvVHgu07gWqd_cH5NuQ

### extract_latest_video
fabric -u https://www.youtube.com/feeds/videos.xml\?channel_id\=UCBB7sYb14uBtk8UqSQYc9-w | fabric -p extract_latest_video
https://www.youtube.com/watch?v=SIzDi6pSD4U (6 days old

### extract_song_meaning
fabric -u https://www.dead.net/song/sugaree | fabric -p extract_song_meaning

