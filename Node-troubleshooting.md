# Add Node.js to PATH on Windows

If you are getting 'node is not recognised' or a similar error, follow these instructions.

## Node is installed but “node is not recognized”

### Add to PATH

1. Press **Start** and search for **Edit the system environment variables**.
2. Click **Environment Variables…**.
3. Under **User variables**, select **Path** → **Edit**.
4. Click **New** and add:

   * `C:\Program Files\nodejs\`
   * `%AppData%\npm`
5. Move these entries **near the top** (above conflicting tools, if any).
6. OK → OK → OK to close all dialogs.
7. Close and reopen git bash, then verify:

   ```sh
   where node
   node -v
   npm -v
   ```

## Quick troubleshooting

* Open a **new** terminal after changes.
* Run `where node` to see which path is used first.

Shout if you want a one-pager PDF with screenshots for students.
