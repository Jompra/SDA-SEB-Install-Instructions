# Add Node.js to PATH on Windows

If you are getting 'node is not recognised' or a similar error, follow these instructions.

## Node is installed but “node is not recognized”

### Add to PATH

1. Press **Start** and search for **Edit the system environment variables**.
2. Click **Environment Variables…**.
3. Under **User variables**, select **Path** → **Edit**.
4. Click **New** and add (as two seperate entries):

   * `C:\Program Files\nodejs\`
   * `%AppData%\npm`
5. Move these entries **near the top** (above conflicting tools, if any).
6. Click OK, OK, OK to close all dialogs.
7. If you already have a gitbash window open, close it first then open or re-open git bash, then verify:

   ```sh
   where node
   node -v
   npm -v
   ```
If you see a filepath for the first one, and some numbers for the second two you are good to go.

## Quick troubleshooting

* Open a **new** terminal after changes.
* Run `where node` to see which path is used first.
