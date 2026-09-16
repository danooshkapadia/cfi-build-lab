# The living dashboard · recipe

What you watched in the Build Lab, written down so you can do it at your desk. About 30 minutes.

## What it is

A one-page dashboard that reads a file every time you open it. Drop a new version of the file in the folder, reopen the dashboard, and it is current. Nobody refreshes anything. Nobody asks anyone for anything.

## The shape

    a file in SharePoint  →  Claude reads it  →  the dashboard shows it
                               (every time you open the dashboard)

The dashboard cannot reach the outside world on its own. Claude reads the file and hands the dashboard the numbers. That is why the file lives in SharePoint, where Claude's Microsoft 365 connector can see it (OneDrive is the same connector and needs no permissions from IT).

## Step 1 · Put a file in SharePoint

Use the sample to start: `cfi-orders-weekly-v1.csv`. Put it in a OneDrive or SharePoint folder you own. Name the folder something you will not rename, for example `Build Lab`. Write the path down. Skills and dashboards point at paths, and moving things breaks them.

## Step 2 · Build the dashboard

Open the Claude desktop app, Cowork, New. Make sure Microsoft 365 shows as connected (Settings, Connectors). Paste the prompt from `dashboard-prompt.md` (it is in the same downloads folder as this recipe). Claude will ask to use the connector once. Say yes. It builds the dashboard and puts it in the Artifacts tab on the left.

## Step 3 · Prove it

Open the dashboard. Note the top number. Close it.
Now put `cfi-orders-weekly-v2.csv` in the same folder, renamed to `cfi-orders-weekly-v1.csv` (replace the old one).
Open the dashboard again. The number changed.

That is the whole idea. The file is the only thing that moves. The dashboard follows.

## Step 4 · Make it yours

Replace the sample file with a real export from your system: Epicor, the CRM, a weekly report someone already sends you. Same file name, same folder, same columns if you can. Then tell Claude what the columns mean and ask it to rebuild the tiles.

If someone already sends you a weekly spreadsheet, ask them to save it to the folder instead of emailing it. That is the last time anyone has to send you a report.

## Where people get stuck

| Stuck on | The move |
|---|---|
| "Can't find the file" | Check the folder name and file name match exactly. Then check Settings, Connectors, Microsoft 365 is connected. Reconnect if in doubt. |
| Dashboard shows old numbers | Close it fully and reopen. It reads on open, not while it sits there. |
| Tried to give it an Excel file | Save as CSV first. Claude reads CSV and text reliably through the connector. Formatted Excel and PowerPoint do not travel well. |
| Want it emailed | Ask for the dashboard to also save an HTML file to the folder each week, and email yourself the link. Claude can stage an email draft with a link; it will not attach files. |
| Want it to look like a report | Ask for an HTML file, not a CSV. Anything in code formats well. |
