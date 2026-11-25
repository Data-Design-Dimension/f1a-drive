# f1a drive app
Mobile app connects F1 Academy drivers to the fans they need to grow, and inspires the next generation of women.

Audio-first prototype: F1 Academy driver records a voice note, fans listen and vote on what she talks about next.

## Disclaimer
This project and its maker are not currently affiliated or endorsed by F1 Academy or Formula One Group in any way, although the opportunity to build with them would be welcome! This is a grass-roots driver-inspired fan-initiated experienc.

## Run

Open index.html in a browser. Fan tab: play sample note, vote on themes. Driver tab: see themes, get script starters, record a note (mic permission needed).

## Voting model

	•	Each vote has weight 0.5^(hours_ago / 48). Votes lose half their weight every 48 hours.
	•	Theme score = sum of weights.
	•	Bubble diameter = 62 + 96 * sqrt(score / max_score) px. Square root keeps bubble area roughly proportional to votes.
	•	Pulse speed also scales with score (top themes pulse fastest).
	•	Production rules to add: one vote per fan per theme per day, bot limits, minors protections (no open DMs, moderated replies).

## Safety

	•	Listen only when parked or as a passenger. Audio-only mode once a vehicle is moving.
	•	Many fans and some drivers are minors: parental consent, no location sharing, moderated voice.
	•	"Demo Driver" is a placeholder. No real driver content or team/series audio is used.

## Status

Prototype only. Data is in memory and resets on reload.
