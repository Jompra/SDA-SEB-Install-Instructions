## Install pgAdmin 4 and Connecting to a Local PostgreSQL Database

### 1. Download pgAdmin 4

* Download PGAdmin Here: [https://www.pgadmin.org/download/](https://www.pgadmin.org/download/)
* Select your operating system (Windows, macOS, or Linux).
* Download and run the installer.

### 2. Install pgAdmin 4

* Follow the installer prompts (default settings are fine for most people).
* When installation finishes, launch **pgAdmin 4**.
* The first time you open it, pgAdmin will ask you to set a **master password** Make sure you make a not eof it and do not forget it.

### 3. Check PostgreSQL is Running Locally

* If you installed PostgreSQL already, make sure the PostgreSQL service is running:

  * **Windows**: Look in *Services* for “PostgreSQL”.
  * **macOS/Linux**: Run `psql --version` or `pg_ctl status` in the terminal.

By default, PostgreSQL listens on `localhost` (127.0.0.1) and port `5432`.

### 4. Add a Connection in pgAdmin

1. Open pgAdmin 4.
2. In the left-hand **Browser** panel, right-click **Servers** → **Register** → **Server...**.
3. In the **General** tab, give it a name (e.g., *SEB-DB*).
4. Go to the **Connection** tab and enter:

   * **Host name/address**: `localhost`
   * **Port**: `5432` (Should be in as default)
   * **Maintenance database**: `postgres` (default)
   * **Username**: `postgres` (unless you set another user when you installed On Monday)
   * **Password**: your PostgreSQL password (set during installation).
5. Click **Save**.

### 5. Verify the Connection

* Expand the new server in the Browser tree.
* You should see **Databases**, **Schemas**, and so on.
* You’re now connected to your local PostgreSQL database through pgAdmin.

If you see your database in the left hand panel, you are 100% set up and ready to go.

If you face a hickup we will make a note and then offer an alternative solution during the course. For now don't worry about it.
