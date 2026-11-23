# Sift

Upload an image and it turns into a field of drifting particles. Everything runs in the visitor's browser (WebGL 2): images are never uploaded to a server and nothing is stored.

## Deploy to Vercel

**Option A: command line**

    npm i -g vercel
    cd sift-vercel
    vercel          # first run: log in, accept the defaults (no framework, no build command)
    vercel --prod   # gives you the public URL to share

**Option B: GitHub**

1. Push this folder to a new GitHub repo.
2. On vercel.com: Add New → Project → import the repo.
3. Framework preset: **Other**. Leave the build command and output directory empty. Deploy.

Each push to the repo redeploys automatically.

## Controls

- Wind, Burst, Form, Relief: how particles drift, burst, settle and how deep the image is
- Flow pad: drag the middle to move the line, drag an end to turn it, tap a side to switch which side streams away
- Top left: download the current frame as a PNG
- Space / arrow keys: next image · H: hide the interface · B: light/dark
