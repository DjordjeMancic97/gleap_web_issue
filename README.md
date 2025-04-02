# gleap_issue

Video link https://files.fm/u/x52p9dae29

Sample project demonstrating misc gleap errors on Flutter Web

Some error messages which are showing up:

- Web app stuck on loading, flutter stuck on "waiting for connection from debug service on Chrome"
  Inside Chrome dev tools console there is huge error "Uncaught Error: Mismatched anonymous define() module: ...."
Refreshing the page fixes the issue.

- Sometimes app will start fine - however same message from above case is present in console and Gleap is not initialized, refreshing the page also fixes this
- App will start fine however exception on Flutter side appears "TypeError: Cannot read properties of undefined (reading 'Gleap')"
  There are multiple variations of this exception sometimes its property "Gleap" sometimes its any of the functions specified inside <script> in "index.html" like "on", "initialize", "open" etc.
Again solution seems to be refreshing the page.

None of the issues are present after Gleap is removed from pubspec.yaml
