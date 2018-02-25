1.0.4:
- Shift-Esc cycles focus through 3 page areas: videos, masthead (search), content below video
- Mousewheel over player ajusts volume
- Switching to fullscreen focuses the player (enables Up/Down volume control, Left/Right jump)
- player, video, comment focus is visualized (box-shadow style) on both classicUI and materialUI
- clarify capturing event handlers captureKeydown(), captureFocus(): run at earlier phase than onKeydown()
- support embedded player, cache playerElem; channel pages have a second player, that is unsupported yet and has the default behaviour
- documented shortcut behaviour and sources

1.0.3:
- added keydown handler: Esc switches focus between player and page, Space pauses anywhere on page, except textboxes
- arrow keys are redirected from sliders directly to the player, no special behaviour when progressbar/volume slider is focused
- therefore no more need to steal focus from player controls when clicked
- tabindex set for player frame and removed for .caption-window

1.0.2:
- support both classic and material design (polymer) html5 player
- allow focusing by TAB: listen for mousedown & focus events to identify focusing by mouse
- added css: translucent lightblue background for focused element to aid TABing

1.0.1:
- support classic html5 player (#movie_player element is constructed later than userscript loaded)
- also broke material design (polymer) html5 player support
- @match *://

1.0:
- support material design (polymer) html5 player
