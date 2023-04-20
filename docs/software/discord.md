---
hide:
 - toc
 - path
 - title
---

## Debloat Discord 
Source: fernbacher

- Browse to your local AppData folder (type in `%LOCALAPPDATA%`) and browse to your Discord installation, then the `modules` folder.
- Keep only `discord_desktop_core-1`, `modules-1`, `utils-1`, `voice-3`. You may want to keep other modules too that you might need.
- Now go up a folder and go into the `locales` folder.
- Keep only the language you use and I advise to keep `en-US.pak` to prevent issues (from personal experience).
- This method should continue to work whatever the Discord version, feel free to fix anything in a pull request though.
- **⚠ Warning: With each Discord update, the modules & locales will come back! This is why it is advisable to use Discord web or a client alternative like [WebCord](https://github.com/SpacingBat3/WebCord).**
`With the help of he3als`

---

## Extra 

Use [OpenAsar](https://openasar.dev/)

<details>
  <summary>CSS Customization</summary>
  
```
/* Hide Gift Button in chat box */
button[aria-label="Send a gift"] {
    display: none;
}
/* Hide Nitro Tab in Friends Menu */
.channel-1Shao0.container-32HW5s[aria-posinset="2"] {
    display: none;
}
/* hide nitro boost banner */
div.container-2giAcK[tabindex="0"] {
    display: none;
}
/* hide nitro boost banner */
div.container-2giAcK[tabindex="0"], div.container-2giAcK[tabindex="0"] + div {
    display: none;
}

/* Compact channels catégories */

:root {
    --category-spacing: 0px;
    --channel-spacing: 4px;
}

.containerDefault-3TQ5YN, .containerDragAfter-1J_-1V, .containerDragBefore-ei4h1m, .containerUserOver-3woq86 {
    padding-top: var(--category-spacing);
}

.mainContent-20q_Hp {
    padding: var(--channel-spacing);
}

/* Slidy Members */
[class*="membersWrap-"] [class*="membersGroup-"] {
    margin-right: auto;
    width: 57px;
    text-overflow: clip;
    direction: rtl;
    word-spacing: 1000px;
}
[class*="membersWrap-"]:hover [class*="membersGroup-"],
[class*="membersWrap-"]:focus-within [class*="membersGroup-"] {
    width: 100%;
    margin: 0;
    direction: ltr;
    word-spacing: unset;
    text-overflow: ellipsis;
}
.membersWrap-3NUR2t{
  min-width: 0 !important; 
}
.members-3WRCEx {
  transition: 250ms ease all;
  width: 64px !important; 
}
.members-3WRCEx:hover {
  width: 64px !important;
}
.membersWrap-3NUR2t:hover .members-3WRCEx{
  width: 245px !important;
}
/* Minified Search Bar */ 

:root {
    --transitionspeed: 0.25s;
}

.search-2Mwzzq:not(.open-1F8u2c) .searchBar-jGtisZ {width: 27px; transition: var(--transitionspeed); background-color: transparent;}
.search-2Mwzzq:not(.open-1F8u2c):hover .searchBar-jGtisZ {width: 170px; background-color: var(--background-tertiary);}
.search-2Mwzzq:not(.open-1F8u2c) .iconContainer-1RqWJj {transform: scale(1.3); transition: var(--transitionspeed);}
.search-2Mwzzq:not(.open-1F8u2c):hover .iconContainer-1RqWJj {transform: scale(1);}
.search-2Mwzzq:not(.open-1F8u2c) .icon-18rqoe {color: var(--text-normal);}
.search-2Mwzzq:not(.open-1F8u2c):hover .icon-18rqoe {color: var(--text-muted);}
/* Channel Names Capitalized */

.channelName-3KPsGw {
text-transform: capitalize;
}
```
</details>

---
## Altenative Client

WebCord [**Link**](https://github.com/SpacingBat3/WebCord)

Ripcord[**Link**](https://cancel.fm/ripcord/)

