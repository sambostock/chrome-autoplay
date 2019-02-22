# Chrome Autoplay Override Test

To test,
  - clone repo
  - run `python -m SimpleHTTPServer 12345` or similar to serve the file
      - any port can be used, just pick one you wouldn't already have a high Media Engagement Index on
  - visit `http://localhost:12345/autoplay-override-test.html` in your browser and click to interact with the page
  - visit `chrome://media-engagement/` and look for `localhost:12345`
      - note this will only update after you close the other tab, ending the session
      - refreshing the other tab does not end the session
  - the Media Engagement Index shoud slowly go up, eventually passing the `high` threshold
