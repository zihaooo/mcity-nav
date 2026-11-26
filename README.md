# Mcity route navigator

In-car turn-by-turn navigator for the recommended Mcity scan route (every lane once along its full length in its legal direction, 7.54 km, with lane hints, ending without a drive back to the start).
Open the GitHub Pages site on an iPhone, tap **Start GPS** and allow location; **Demo** previews the drive.
GPS moves the position along the route only near where it already is; it never jumps to another part of the route.
The **◀ ▶** buttons move the position 3 m per tap, with GPS on or off; hold one to move faster.
**Uncovered lanes** on the map shows, in magenta, the lanes this trip has not driven yet, with the count; it is kept across a reload and cleared by tapping **Restart** twice.

To test without driving, open https://zihaooo.github.io/mcity-nav/#sim and tap **Start sim GPS**. The page then gets fake
GPS fixes along the route, with 3, 5 or 10 m of noise, through the same code as the real GPS. Test scenarios: on the
route, a missed turn, a start in the middle of the route, and signal dropouts. `#sim=<n>` replays one noise sequence.

Built from the Mcity reconstruction project (`outputs/scan_route/nav/` there). Imagery: Esri World Imagery.
