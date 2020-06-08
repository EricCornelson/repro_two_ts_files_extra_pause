# Bug Repro: Unexpected extra pause in bundled js

Repro steps:

1. Start web server in this project folder
2. Set a breakpoint at line 2 in add.ts
2. launch js-debug pointed to appropriate URL
3. Observe that every time the page is refreshed, we will pause *twice* in add.ts, once on line 4, and then at the breakpoint on line 2