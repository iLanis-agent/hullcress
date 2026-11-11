# Hullcress 1.0 TEST
Native Android convex hull corner recognition puzzle. Android 8+ min26/target35. Package com.gg007.hullcress.

## Rules
Known convex-hull recognition adaptation. Ten fixed dots are shown on a coordinate grid. Tap exactly the outer corners that a tight rubber band around ALL ten dots would touch. Leave every interior dot out, then press CHECK HULL. Selecting all dots is not a solution. No three points are collinear in any shipped puzzle, so there are no ambiguous straight-edge dots. Twelve original ten-point sets, each with one hull vertex set and 5-7 outer corners. Order of selection does not matter. Gold boundary appears only after a correct answer. Undo/reset, GG007 menu/site/privacy and saved palette/optional point letters. Tap the title or Android Back for menu.

## Download and status
https://mega.co.nz/#!UZEilBKZ!SiRDirxIfFBjesOts-GpWWgwxOZySSW0Ht3hfkrwzJQ
APK 20974 bytes; SHA256 86b817b5b9a05c1d321faa96f61442d6f31cec08e9a7a9639cd6227eefc1185a. Original certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions, original GG007 icon unchanged. Anonymous downloaded bytes match.

## Checks
Seed 1031111 produces twelve distinct ten-point sets; no duplicate points or collinear triples, and pairwise coordinate separation at least two grid units. Independent supporting-line edge enumeration matches the production sorted monotone-chain hull. All 1024 subsets per level, 12288 total, verify exact-set acceptance. Another 122880 dot-toggle/undo transitions verify restoration; 1000 random general-position sets independently compare the two hull algorithms. Empty/all-point rejections, collinear endpoint-only policy, invalid mask/point/level bounds, duplicate validation and reset are checked. All twelve actual drawing-adapter dot/CHECK tap-solves, solved locks, actual NEXT, undo/reset/levels/title-menu/privacy/saved palette-labels pass. Twenty drawing previews inspected, not phone screenshots. Phone runtime, performance, browser handoff QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
All 234 prior studio descriptions reviewed. The 803 legacy registry is byte-identical to its previously reviewed baseline; convex-hull/extreme-point/rubber-band/enclosing-point scan found no matching mechanic. Hullcress classifies the extreme vertices of a planar point set, using geometric orientation and an exact corner-set goal. Knotcress moves graph nodes to uncross fixed links; Anglewren draws an all-symbol loop constrained by angle types; Graftcress chooses minimum-cost graph edges. Those do not classify outer vs interior points or construct a minimum enclosing convex boundary. Known convex hull, not a globally new algorithm. Original seeded point sets, native implementation and point-map illustration. Six university, library-documentation and programming-community sources checked for definition and collinear policy; no source implementation copied.

## Build and tests
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/merge-test src/com/gg007/hullcress/Board.java BoardTest.java then java -cp /tmp/merge-test com.gg007.hullcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret included. adapter/android is a Java2D drawing adapter used with HullAdapterTest.java, not an Android runtime.

## Privacy and branding
Hullcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, point letters and solved-level marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon and studio https://ilanis-agent.github.io/gg-007-gaming/.

## Preservation and publishing
Complete source/APK, exact cumulative 235-card studio and publishing fragments privately preserved:
https://files.instinct.com/9iqwyyevgvuw-hullcress-source-archive
https://github.com/iLanis-agent/hullcress holds README only, full Git source pending. All four existing studio includes and prior card bytes unchanged. Pages settings untouched. Both live sites verified separately.

## Rule sources
https://www.cs.umd.edu/class/fall2023/cmsc754/Lects/lect02-hulls.pdf
https://commons.apache.org/proper/commons-math/javadocs/api-3.6.1/org/apache/commons/math3/geometry/euclidean/twod/hull/MonotoneChain.html
https://ti.inf.ethz.ch/ew/lehre/CG12/lecture/Chapter%203.pdf
https://cp-algorithms.com/geometry/convex-hull.html
https://mtuann.github.io/competitive-programming-cpp/topics/geometry/convex-hull/
https://sandeepswain.dev/citadel/cp/convex-hull-construction
