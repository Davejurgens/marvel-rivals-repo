# Setting up your development environment tutorial

![alt text](../media/Cover_8.png)

These are the steps you must do before you can run
the tutorials for the **Marvel Rivals Ranking service**.

Expect this preparation to take about 20 minutes to complete.

## Step 1: Preparing for the tutorials

The following instructions describe how to prepare for running the tutorials on Windows.
For information about how to prepare MacOS for the tutorials, visit the [MacOS installation guide](macos-installation).

### To complete the tutorials in this section, you need the following:

* A [GitHub account](https://github.com)
* The following software on your development system:
    * [Git](https://docs.github.com/en/get-started/quickstart/set-up-git) (for the command line)
    * [GitHub Desktop](https://desktop.github.com) (optional)
    * A fork of the [Marvel-Rivals-repo](https://github.com/Davejurgens/marvel-rivals-repo/tree/main)
    * A current/LTS version of [node.js](https://nodejs.org/en/)
    * A current version of [json-server](https://www.npmjs.com/package/json-server)
    * A current copy of the database file. You can get this by syncing your fork.
    * The [Postman desktop app](https://www.postman.com/downloads/). Because you run the **Comic Database Service** on your development system with an `http://localhost` hostname, the web-version of Postman can't perform the exercises.

## Step 2: Test your development system

Create and checkout a test branch of your fork of the comic-database-service repo. You can download these from the [Marvel-Rivals-repo](https://github.com/Davejurgens/marvel-rivals-repo/tree/main).

To download each file:
1. Move your cursor over the filename and select the link that appears.
2. Locate the download button on the top right corner of the panel, indicated by a downward arrow, and click it.
3. Repeat this process for the `db.json` file and one of the startup scripts: `start-server.sh` for macOS and Linux 
   or `start-server.bat` for Windows.

## Step 3: Run the JSON server

1. Navigate to the directory where you downloaded db.json and the start scripts.
2. On Windows, double-click the `start-server.bat` file to start the service. On macOS or Linux, open the terminal, 
   `cd` <directory name> where you downloaded the files, and type `./start-server.sh`. That runs the script in the 
   current directory. If that doesn’t work, type `json-server db.json`. You should see some text to show the service is running:

    ```
     macBook:api <username>$ json-server -w db.json

     \{^_^}/ hi!

     Loading db.json
     Done

     Resources
     http://localhost:3000/duelists
     http://localhost:3000/strategists
     http://localhost:3000/vanguards

     Home
     http://localhost:3000

     Type s + enter at any time to create a snapshot of the database
     Watching...
    ```

3. If your development system is installed correctly, you should see the service start and display the URL of the service: `http://localhost:3000`.

2. Make a test call to the service.

    ```
    curl http://localhost:3000/duelists
    ```

3. If the service is running correctly, you should see a list of superheroes from the service, such as in this example.

   ```
   "duelists": [
    {
      "superhero_name": "Scarlet Witch",
      "damage_type": "Projectile, Area of Effect",
      "difficulty": "3",
      "id": 1
    },

4. If you don't see the list of superheroes, or receive an error in any step of the procedure, investigate and correct the error before continuing. Some common situations that cause errors include:

   1. You mistyped a command.
   2. You aren't in the correct directory.
   3. A required software component didn't install correctly.
   4. A required software component isn't up to date.

If you see the list of comic books from the service, you're ready to do the tutorials.
