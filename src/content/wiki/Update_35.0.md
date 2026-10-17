---
title: "Update 35.0"
section: "Updates"
cats: ["Updates"]
---
**[OpenFront](/OpenFront.io) v35** — The progression update: player [levels and XP](/Levels_and_XP) with prestige, Ranked FFA and Clan Wars, a seekable replay viewer, much smarter [nations](/Nations), faster quick chat and emoji, nukes that [annex](/Annexation) again, lobbies bigger than 125 players, and twelve new maps.

Released **October 16th 2026** (v0.35.0), followed by v0.35.1 and v0.35.2 the same day.

# 📦 OpenFront v35 Changelog {#OpenFront_v35_Changelog}

## ⭐ Overview {#Overview}

- **Player levels & progression** — Every game now earns XP, shown on the end-of-game screen. Level badges appear across the lobby, player panel, leaderboard and clan lists. At level 100 you can Prestige, up to P10 and then Legend. Profiles get a Progression tab with a reward track that pays Plutonium every 25 levels. Subscribers level faster, up to +100% for Sovereign. See [Levels and XP](/Levels_and_XP).
- **Ranked FFA and clan wars** — Two new [ranked](/Ranked) queues: Free For All (4–10 players matched by ELO, last player standing wins) and Clan Wars (your [clan](/Clan) vs. up to three others, 2–5 a side, the clan gains or loses rating). Ranked now needs a trusted account, and the clan leaderboard gets an ELO column.
- **Meta** — Your first few [ports](/Port) and [factories](/Factory) now spawn [trade ships](/Trade_Ship) and [trains](/Train) faster. More buildings still means more trade overall.
- **Replay viewer** — Replays can seek. The game is processed once in your browser, then any point on the timeline is a ~20 ms jump. Finished games open in the viewer from the game history. (Disabled by default at launch and rolled out over the following week or so.)
- **Smarter nations** — [Nations](/Nations) play more like the humans who win: they save later and keep building, fortify borders before attacking, send 1% beachhead boats and follow up by land, defend against landings, retaliate properly, aim nukes at land instead of water and [fallout](/Fallout), nuke back, and in FFA gang up on a runaway leader. Easy nations keep their old behaviour.
- **Faster chat and emoji** — R opens quick chat on the player under your cursor and one click sends a phrase. F opens a redesigned, grouped emoji menu with a Favorites row you fill by drag and drop and fire with Q W E A S D. The top player panel gets chat, emoji, alliance (K/L), target (N) and boat (B) buttons. Select-all-warships moves from F to X. See [Controls](/Controls).
- **Nukes annex again** — Nuking an arm off someone's territory hands the cut-off piece to the surrounding enemy again. It had stopped working for most coastal empires. See [Annexation](/Annexation).
- **Bigger lobbies** — The 125-player cap is gone. Lobby size now comes from the map, so [The Box](/The_Box) fits 210, [Alps](/Alps) 185 and [Middle East](/Middle_East) 170.
- **New maps** — [Madagascar](/Madagascar) (a Baikal-style Nuke Wars map), [Horn of Africa](/Horn_of_Africa), [Vancouver Island](/Vancouver_Island), [Cape of Good Hope](/Cape_of_Good_Hope), [Canary Islands](/Canary_Islands), [Bab el-Mandeb Strait](/Bab_el-Mandeb_Strait), [Rio de Janeiro](/Rio_de_Janeiro), [Pulicat Lake](/Pulicat_Lake), [Benelux](/Benelux), [New Zealand](/New_Zealand) and [Brain Rot](/Brain_Rot), plus [Ommatrypta](/Ommatrypta) for Halloween.
- **Faster homepage** — The homepage's first download is a third of what it was (661 KB → 220 KB gzipped). The game client, store and every modal load on demand.

## ☢️ Gameplay & Balance {#Gameplay_Balance}

- Removed the 125 player cap from public lobbies; size now comes from the map's land, and [Alps](/Alps) and [The Box](/The_Box) appear more often — **FloPinguin**
- [Annex](/Annexation) land a nuke cuts off from the main body; this had stopped working whenever the main body touched the coast — **Lewis**, **JB940**
- Humans can send up to 5 emojis per recipient per 5 s (was 1) — **Evan**
- Dropped attacks with an invalid troop count instead of kicking the player; about 50 players a day were losing their game to it — **Evan**
- Each player's spawn tile is recorded in their stats, for future per-map spawn heatmaps — **Lewis**
- Meta: faster [trade ships](/Trade_Ship) and [trains](/Train) for players with only a few [ports](/Port) or [factories](/Factory) (a 1-port player sends a ship every ~8 s instead of ~12 s); the boost fades out by 6 levels and replaces the old fleet-size boost — **Evan**
- "Stop Trading with All" is now "Stop Trading with Enemies" and keeps [trade](/Trade) with your allies — **FloPinguin**
- Fixed trains not earning [gold](/Gold) at a station built on the stretch of track they were already on — **cazlabIO**
- Fixed [MIRVs](/MIRV) aimed at unclaimed land: no more "Player with id null not found" error, and if someone takes the tile before launch, they're the one warned and targeted — **VariableVince**

## 🤖 Nations {#Nations}

- [Nations](/Nations) play more like winning humans: later saving, continuous building, [defense posts](/Defense_Post) behind the front, [bots](/Bots) annexed by walling them in, nukes on bordering rivals and nuking back, [MIRVs](/MIRV) on reachable targets, and team nations backing up teammates — **FloPinguin**
- Smarter nukes: no two nations nuke the same spot, no blasts wasted on water or [fallout](/Fallout), [atom bombs](/Atom_Bomb) on small islands, collateral on non-allies in FFA, never own or allied enclaves — **FloPinguin**
- 1% beachhead boats on Hard and Impossible, followed by a land attack the tick they land; Medium and up stop saving for nukes before three [cities](/City) — **FloPinguin**
- Retaliation, naval warfare and pressure on a runaway FFA leader: nations answer attacks before saving, route boats around [warships](/Warship), send warship squads at blockades, and don't sail past 300/500 tiles — **FloPinguin**
- Nations defend against boat landings at the beachhead and stop stacking defense posts on top of each other — **FloPinguin**
- Nations keep donating troops to fighting teammates after the game is decided, celebrate wins with an emoji, and only one nation mocks a [traitor](/Traitor) instead of all twenty — **FloPinguin**

## 🏆 Ranked & Clans {#Ranked_Clans}

- [Ranked](/Ranked) Free For All: 4–10 players matched by ELO, continent maps, 20 minute timer, ends when one human is left — **Evan**
- Ranked Clan Wars: clan-sized team games, 2–5 a side, up to four clans, rated per clan — **Evan**
- Ranked is limited to trusted accounts, with lock icons on the Ranked button and modal — **Evan**
- [Clan](/Clan) leaderboard gets a sortable ELO column — **Evan**
- Clan browser: a fair per-player random order by default (no more "AAA" clans at the top), sort options, and paid clan boosts for featured placement — **Lewis**
- Clan browser: sort by Oldest, Richest or Lowest win score, and filter to open or invite-only clans — **Lewis**
- Clan wars queue shows how many from your clan are waiting — **Evan**
- Clan Members list shows each member's clan wars ELO contribution, with a sort for it — **Evan**
- Clan tags come from the clan wars assignment — **Evan**
- Ranked alert redesign — **cazlabIO**

## 📈 Levels & Progression {#Levels_Progression}

See [Levels and XP](/Levels_and_XP) for the full XP formula.

- Player levels: a level badge across the UI and an XP reveal on the end-of-game screen, source by source, with level-ups — **Lewis**
- A provisional XP figure the moment you're out, reconciled with the server's when the game ends — **Lewis**
- Profile cards, and the prestige flow at level 100: a hold-to-confirm screen and a full-screen ceremony, P1 to P10 then Legend — **Lewis**
- Progression tab, reward track, profile links and sharing, and end-of-game rewards — **Lewis**
- Level badges in the lobby list, in-game player panel, ranked leaderboard (prestiged players and Legends only) and clan member lists — **Lewis**
- Privacy settings: hide your level from other players, and keep your profile out of search engines — **Lewis**
- Level Plutonium is held until your account is trusted, and the rewards list says so — **Lewis**
- New level badges: each prestige rank has its own unit icon, tier colour and rim gauge (Iron to Champion, then Legend), with a glow on P5, P10 and Legend and sparkles from P8. Share cards match — **Lewis**
- Your Account has a Progression tab: the reward track with Claim all, prestige history and milestones — **Lewis**
- Your level shows the XP from games still being scored, marked provisional, and it stacks across back-to-back games until each one is confirmed — **Lewis**
- Subscriber XP boost: Vanguard +25%, Warlord and Steam Plus +50%, Sovereign +100% — **Lewis**
- Levels take about 20% more XP: level 1 to 100 is now 44,690 XP (was 37,300). Nobody loses a level — **Lewis**

## 🧑‍🤝‍🧑 Lobby & Social {#Lobby_Social}

- Quick chat: R opens it for the player under your cursor, phrases are one-click chips grouped by category, and phrases that name a player open a ranked picker — **Evan**
- Emoji menu redesign: grouped sections, a Favorites row with Q W E A S D hotkeys, F to open, and batch sending — **Evan**
- Player panel shortcuts: Send/Break alliance (K/L), Target (N) and Boat attack (B), each shown only when it applies — **Evan**
- Quick chat: a Recent section and phrase search — **FloPinguin**
- Eight new quick chat phrases ("Betray [P1]!", "Build SAMs!", "Send gold to [P1]!", …) plus "Attack the crown!" — **Lewis**, **Evan**
- See what a player is wearing in their info panel, with store links for anything you don't own — **CodingSelim**
- Hosts can set a player limit (2–1000) on an unlisted private lobby — **Lewis**
- Public [team](/Teams) lobbies show the lobby ID and copy button too, so you can share the link or keep the game ID (not in FFA, to discourage teaming) — **FloPinguin**
- A larger map preview and compact setting tags in the lobby waiting view — **Gio Marco Baglioni**
- Duos / Trios / Quads labels are back, and the same lobby reads the same everywhere — **FloPinguin**
- Fixed the team name being untranslated in the win message — **VariableVince**
- Fixed quick chat keeping a stale player selected when switching phrases — **LoSt543215543**
- Alliance request confirmations keep the clan tag in the name — **LoSt543215543**
- Fixed Alt+click on an emoji sending it to whoever was under the cursor — **LoSt543215543**
- Fixed double colons on localized lobby badges in CJK languages — **LoSt543215543**
- Centred the kick button icon in the lobby player list — **LoSt543215543**

## 🎞️ Replays {#Replays}

- A replay viewer that can seek: processed once in your browser, ~20 ms per seek, verified against the hashes the live clients recorded — **ArtZab0**
- Viewer follow-ups: playback keys ignored behind settings, no event flood when switching followed players, unverified replays flagged, backward seek fixes gold/s — **ArtZab0**
- Game state snapshots: the whole simulation can be saved at any tick and restored with identical hashes, for pause/resume, forks and replay seeking — **Evan**

## 🎛️ Graphics, UI & Quality of Life {#Graphics_UI_Quality_of_Life}

- The in-game menu now lists the game's modifiers, disabled units and host cheats, in replays too — **FloPinguin**
- HUD background opacity slider in Settings → Graphics, so the leaderboard and panels hide less of the map — **MRGhust**
- Halloween homepage theme: orange and purple, pumpkin cursors, a blood moon on the map cards (homepage only, never in game) — **Restart**
- The Halloween theme runs from Oct 25 through Nov 1, and a Settings toggle turns it off — **Evan**, **Josh**
- Halloween homepage cleanup: brighter lobby buttons, natural map thumbnail colors, and no more cobweb over the modal back arrow — **Restart**, **VariableVince**, **Evan**
- Fixed the white strip under the Steam store widget on the dark homepage and win modal — **Lewis**
- Drag to dismiss in-game toasts, which matters on phones where a long error covered the map — **MRGhust**
- The structure preview now sits where the building will actually go when you're placing it near another (made optional in v0.35.2, see below) — **MRGhust**
- Mobile attack ratio control shows the troop count, not just the percentage — **Kinatic11**
- Arrow and zoom keys are now real keybinds, so assigning them elsewhere no longer fires both actions — **VariableVince**
- Fixed Escape closing the whole Settings modal when cancelling a keybind capture — **LoSt543215543**
- Fixed Mac Ctrl+click opening the radial menu and attacking at the same time — **devynlynch**
- Fixed a soft-lock where clicking a build icon opened the radial menu over the HUD — **torturado**
- Fixed a crash when releasing a build just past the map edge — **Evan**
- Signed-out players are told how to get skins, crowns and effects in the inventory — **MRGhust**
- Fixed your equipped cosmetics resetting when you come back to the site — **LoSt543215543**
- Localized unit names in "missile intercepted" and "unit destroyed" events — **Aotumuri**
- Incoming unit messages are now translatable — **VariableVince**
- Muted sound effects no longer load and play silently in the background — **Alexandre**
- Cosmetic and currency pack names are capitalized in the store — **LoSt543215543**
- Tutorial gives a general reason to ally ("Allies secure your borders") — **FloPinguin**
- Steam prompts say "Buy on Steam" — **LoSt543215543**
- Translation updates (mls v5.17–v5.20) — **Aotumuri**

## 🗺️ Maps {#Maps}

### New Maps {#New_Maps}

<table class="wikitable">
<tbody><tr>
<th>Map</th>
<th>Description</th>
<th>Author</th></tr>
<tr>
<td><b><a href="/Madagascar" title="Madagascar">Madagascar</a></b> ☢️</td>
<td>A dedicated Nuke Wars map: two equal landmasses across the Mozambique Channel, set in the 80s</td>
<td><b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Horn_of_Africa" title="Horn of Africa">Horn of Africa</a></b> 🏴‍☠️</td>
<td>A pirating chokepoint off Somalia and an inner water system from the Nile to Lake Victoria</td>
<td><b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Vancouver_Island" title="Vancouver Island">Vancouver Island</a></b> 🌲</td>
<td>30+ nations from the Pacific Northwest</td>
<td><b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Cape_of_Good_Hope" title="Cape of Good Hope">Cape of Good Hope</a></b> ⛵</td>
<td>A large bay with one chokepoint, plus historical South African flags</td>
<td><b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Canary_Islands" title="Canary Islands">Canary Islands</a></b> 🏝️</td>
<td>An island map with shortened crossings, high in team rotation</td>
<td><b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Bab_el-Mandeb_Strait" title="Bab el-Mandeb Strait">Bab el-Mandeb Strait</a></b> ⚓</td>
<td>A balanced two-team map set in the early 1960s, with the region's flags</td>
<td><b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Rio_de_Janeiro" title="Rio de Janeiro">Rio de Janeiro</a></b> 🏖️</td>
<td>Guanabara Bay, 30 nations from Rio's neighbourhoods and municipalities</td>
<td><b>Renan Scarpin</b></td></tr>
<tr>
<td><b><a href="/Pulicat_Lake" title="Pulicat Lake">Pulicat Lake</a></b> 🌊</td>
<td>A lagoon with a single sea entrance, and a pirate island in the door</td>
<td><b>Panindhra Tallapudi</b></td></tr>
<tr>
<td><b><a href="/Benelux" title="Benelux">Benelux</a></b> 🌷</td>
<td>Belgium, the Netherlands and Luxembourg</td>
<td><b>Niels K.</b>, <b>RickD004</b></td></tr>
<tr>
<td><b><a href="/New_Zealand" title="New Zealand">New Zealand</a></b> 🥝</td>
<td>Traditional Māori tribes as nations, with the country's regions as 80+ more, on a medium-sized map for the Oceania players</td>
<td><b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Brain_Rot" title="Brain Rot">Brain Rot</a></b> 🧠</td>
<td>Here to stay; boosted in the public rotation for Halloween</td>
<td><b>PatrickPlaysBadly</b>, <b>VariableVince</b>, <b>RickD004</b></td></tr>
<tr>
<td><b><a href="/Ommatrypta" title="Ommatrypta">Ommatrypta</a></b> 🎃</td>
<td>Halloween only; boosted in the public rotation for the holiday</td>
<td><b>PatrickPlaysBadly</b>, <b>VariableVince</b>, <b>RickD004</b></td></tr></tbody></table>

### Map Improvements & Fixes {#Map_Improvements_Fixes}

- Better terrain for [Pulicat Lake](/Pulicat_Lake) — **RickD004**
- Took v34 maps out of the New category, and lowered [Channel Islands](/Channel_Islands)' FFA rotation — **RickD004**
- Map layers ship as lossy WebP, ~9× smaller, with a Compact variant — **Josh**
- Map generator: crop layer PNGs to the map size like the terrain — **FloPinguin**

## ⚡ Performance {#Performance}

- The game client loads on demand instead of with the homepage: first download 661 KB → 434 KB gzipped — **Evan**
- Homepage modals, the store, the lobby modals, menu audio and news renderer load on demand: 434 KB → 220 KB gzipped — **Evan**
- Replay processing runs on the engine's own worker; the replay worker shrinks from 815 KB to 340 KB — **Evan**
- Fixed the largest client exception in prod (24% of Firefox sessions) in stylesheet loading — **Evan**
- Fixed PWA icons 404ing on every page load — **Evan**

## 🚂 Steam, Desktop & Poki {#Steam_Desktop_Poki}

- OpenFront is now playable on Poki — **Evan**
- [Steam](/Steam) players who subscribe while they still have free days now get those days added to the end of their subscription — **Josh**
- Boot prompts (claim your username, Steam notices) are only counted once you answer them, so a content update mid-prompt doesn't spend your one showing — **Josh**
- Admin-granted subscriptions are told apart from a Steam month, so a comped player isn't told their access came with a Steam purchase — **Lewis**
- The menu theme no longer starts over the gameplay track when a game starts before the audio chunk loads — **Josh**

## 🩹 v0.35.1 and v0.35.2 {#v0.35.1_and_v0.35.2}

Both released October 16th 2026.

- v0.35.1: Profile cards show the clan tag from your latest game instead of your first clan alphabetically — **Evan**
- v0.35.1: Antarctic tribe themes on the Antarctica and Deglaciated Antarctica maps — **RickD004**, **Josh**
- v0.35.1: Hide the store, Steam promos and profile share links on game portals — **Evan**
- v0.35.2: The build preview follows your cursor again, as in v34. The v35 behaviour of snapping it to the tile it will actually be built on is now the **Snap Build Preview** setting in the Gameplay tab, off by default — **Evan**
- v0.35.2: Fixed kicks not removing players who had rejoined the same game from another tab or device — **Evan**

## 🌐 Translators {#Translators}

- **Arabic🇸🇦**: N0ur, Moha & SyntaxPM
- **Bengali🇧🇩**: sheikh
- **Brazilian Portuguese🇧🇷**: theskeleton4393, juliosilvaqwerty5, Vincent & iliya
- **Bulgarian🇧🇬**: Nikola123 & NewHappyRabbit
- **Chinese Simplified🇨🇳**: Moki
- **Chinese Traditional🇹🇼**: SkiRhino & ChAoSUnItY
- **Czech🇨🇿**: Xaelor, erinthegirl & Matouš Adamů
- **Danish🇩🇰**: NiclasWK
- **Dutch🇳🇱**: cldprv, tryout33, Zjefken & Niels
- **Esperanto**: r3ms & Katokoda
- **Estonian🇪🇪**: ramon.o
- **Finnish🇫🇮**: Tanepro193
- **French🇫🇷**: cldprv, gx21, r3ms & Eiwalis
- **Galician**: toldinsound
- **German🇩🇪**: Pilkey, jacks0n, floriankilian, Fibig, TNB & W4lle
- **German (Switzerland)🇨🇭**: originaloha
- **Greek🇬🇷**: pantelispantelidis
- **Hungarian🇭🇺**: ap.ms & Forsan
- **Hebrew🇮🇱**: Goblinon
- **Hindi🇮🇳**: sheikh
- **Italian🇮🇹**: frappa10 & Lollosean
- **Indonesian🇮🇩**: tronsar
- **Japanese🇯🇵**: Aotumuri, daimyo_panda2, gafunuko, kaywb & aki__san__
- **Korean🇰🇷**: Jinyoon & Game_Sushi
- **Macedonian🇲🇰**: Perdiccas
- **Polish🇵🇱**: zibi, RinkyDinky, Rulfam, Kris & Tomasz
- **Persian🇮🇷**: nobodyiran
- **Russian🇷🇺**: Rulfam, Redincon & Shomped
- **Romanian🇷🇴**: GrunoTheGamer
- **Serbo-Croatian🇷🇸🇭🇷🇧🇦🇲🇪**: Vekser & kw3rty
- **Slovak🇸🇰**: extraextra
- **Slovenian🇸🇮**: MotivatedMonkey
- **Spanish🇪🇸**: 6uzm4n & Campos
- **Swedish🇸🇪**: Moha, theangel2, Keevee & torktumlare
- **Tamil**: UniverSoul
- **Toki Pona**: Makonede
- **Turkish🇹🇷**: Toyatak & grassified
- **Ukrainian🇺🇦**: Rulfam
- **Vietnamese🇻🇳**: Hazun06VN

## 🙏 Contributors {#Contributors}

v35 took 25 people. Code, maps, perf, translations, the lot. Thank you:

**Alexandre** · **Aotumuri** · **ArtZab0** · **cazlabIO** · **CodingSelim** · **devynlynch** · **Evan** · **FloPinguin** · **Gio Marco Baglioni** · **JB940** · **Josh** · **Kinatic11** · **Lewis** · **LoSt543215543** · **MRGhust** · **Niels K.** · **Panindhra Tallapudi** · **PatrickPlaysBadly** · **Renan Scarpin** · **Restart** · **RickD004** · **torturado** · **VariableVince** · **wraith4081** · **youtsuho**

## See also {#See_also}

- [Levels and XP](/Levels_and_XP)
- [Ranked](/Ranked)
- [Update 34.0](/Update_34.0)
- [Update History](/Update_History)
