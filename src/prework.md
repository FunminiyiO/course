# Prework

Finish these steps before Class 1 on Tuesday, Oct 27 at 3:00pm ET.

Complete the steps in order (finish all required steps before the 'bonus' part of step 4). Each step ends with a **Done when:** line so you know you're finished.

1. [Install the Claude desktop app](#1-install-the-claude-desktop-app)
2. [Create your n8n account](#2-create-your-n8n-account)
3. [Create your Claude Project](#3-create-your-claude-project)
4. [Late homework excuse: your first build](#4-late-homework-excuse-your-first-build)
5. [Prepare for the first class](#5-prepare-for-the-first-class)

## 1. Install the Claude desktop app

**Why:** Claude is your build partner for every project in this course. Use the desktop app so Claude is one click away while you work in n8n.

1. Go to [claude.ai/download](https://claude.ai/download) and download the app for your computer (Mac or Windows).
2. Install it and open it.
3. Sign in with your Claude account, or create one if you don't have one yet.

**Done when:** you can start a new chat in the desktop app and get a reply.

## 2. Create your n8n account

**Why:** n8n is where you'll build your automations. You'll work in the shared SchoolRunbook workspace, so there's nothing to pay for or install.

1. Look for an email from n8n inviting you to the SchoolRunbook workspace. It goes to the email address you registered for the course with; check spam if you don't see it.
2. Click the link in the email to create your account. Choose **Sign in with Google**, and use the same Google account you'll use for the course.
3. Bookmark the workspace so you can find it in class: <https://schoolrunbook.app.n8n.cloud/home/workflows>

**Done when:** you can log in and see the SchoolRunbook workspace.

## 3. Create your Claude Project

**Why:** a Claude Project keeps all your course chats in one place, and its instructions are read at the start of every chat in it. This enables us to give the project instructions once, so you don't have to rewrite them for every chat.

<div class="video-embed">
  <iframe src="https://www.youtube-nocookie.com/embed/6iQmqVvYNQI" title="Create your Claude Project" allow="encrypted-media; picture-in-picture; fullscreen" allowfullscreen></iframe>
</div>

**Steps**

1. In the Claude desktop app, open **Projects** and create a new project called `SchoolRunbook projects`.
2. Open the project's instructions and paste in the text in the box below. Leave `[Links to be added]` as it is; you'll replace it with your first project's link in step 4.
3. Connect Google Drive so Claude can read your sheets: in Claude's settings, open **Connectors**, find Google Drive, and click **Connect**. Sign in with the same Google account you'll use for the course.

```text
# My automation projects (SchoolRunbook)

## About this project

I'm a participant in SchoolRunbook, a course where K-12 school leaders learn to use AI to automate school operations work. I use this Claude project for all of my course work. Each project is an automation which I build in n8n with your help. My projects will use n8n Cloud and Google Workspace (Gmail, Sheets, Docs, etc.).

I'm new to n8n and may be new to coding. When you give me code, give me the complete code for the node so I can replace everything in it; I won't read or edit the code itself. When working in n8n, tell me exactly what to name each node and exactly which settings to change.

## My automation projects

Here is a list of my projects:

- [Links to be added]

Each project has one guide: a Claude Doc with a Context tab, plus Design and Build tabs once we start building. Read the Context and Design tabs for background, and the Build tab to see what I'm working on. When I come back to a project in a new chat, be sure to read the project guide so we can pick up where we left off.

When I start a new project, I'll paste its context into my message. Create the project's guide, which has three tabs.

### Context Tab

First, create one Claude Doc named after the project, with a Context tab holding my context. If the context is unclear, ask me questions one at a time to make sure you understand what I want to build and why. Put all of this in the Context tab.

Then remind me to add the guide's link to my list of projects above, and give me the line to paste. I update these instructions myself. Never create a second doc for a project.

Then wait while I read the Context tab and edit it, or ask you to. Don't start the Design tab until I tell you to.

### Design Tab

When I tell you to, add a Design tab. The Design tab is the plan, written so another engineer could understand it and build the automation. Keep it short:

- The problem: a few sentences on how the work is done by hand today and what goes wrong, with a link to the Context tab rather than repeating it.
- What the automation does, and what it doesn't do.
- The nodes in order, with one line each on what the node does and why it's needed.
- The rules the automation follows.

Stop, and wait for me to read the Design tab, ask clarification questions, and make edits. When I tell you to do so, create the Build tab.

### Build Tab

The Build tab tracks my progress. It starts with a short list of milestones, each with a checkbox. Below the checklist, write click-by-click instructions for the current milestone only, in this shape:

1. Goal first: one or two plain-language sentences on what this milestone does and why.
2. Steps: click-by-click, with exact node names and settings.
3. My checks: one or two quick checks I do myself in the node's output panel, using the Table view: for example, how many items came out, or what one column shows for one email. I'm learning to read n8n's output, so I should look every time. Never ask me to read JSON by eye or compare many values.

### How we work through a milestone

1. Your checks: once I've done my checks, check anything more detailed yourself (every row's values, all the categories, edge cases). Tell me exactly what to copy from n8n or the sheet and paste to you.
2. Canvas check: ask me for a screenshot of my n8n canvas, and confirm that the nodes are named, ordered and connected as the Build tab says. Point out anything that doesn't match.
3. Save progress: once the canvas check looks good and we confirm the milestone is done, update the Build tab (tick the box; note anything that differed from your instructions, such as node names, settings or surprises), and update the Design tab if anything about the design changed. The doc should always match what I actually built, so I could pick this up in a new chat.
4. Wait: don't write the next milestone's instructions until I say I'm ready.

When something breaks, I'll paste the exact error or output. Tell me the likely cause and the fix, and give me complete replacement code when the code changes.
```

**Done when:** your `SchoolRunbook projects` project has these instructions saved, and Google Drive shows as connected.

## 4. Late homework excuse: your first build

**Why:** this is a practice run of how we'll build in class, on a small project. Claude writes your project guide (Context, Design and Build tabs), and you build the automation one milestone at a time. Along the way you connect Gmail and Google Sheets to n8n.

**Demo video:** coming soon

Use the same Google account you'll use for the course in every step below.

### Make your sheet

1. In Google Drive, create a new blank Google Sheet called `Prework excuse`.
2. In row 1, type these four headers, one per column: Animal, Adjective, School supply, Body of water.
3. In row 2, type one word under each header. The sillier the better.
4. Copy the sheet's link. You'll paste it into the prompt below.

### Start your project guide

1. In your `SchoolRunbook projects` project, start a new chat. Copy the prompt below, replace `[paste link]` with your sheet's link and `[your name]` with your name, and send it.

```text
Let's start my Late Homework Excuse project. Its context is below.

---

## The problem

I'm doing a prework exercise for the SchoolRunbook course. Before class, I need Gmail and Google Sheets connected to n8n, and I want to practice the way we'll build in class on something small and silly.

## What the automation should do

1. Read the words from my sheet.
2. Put them into a short, formal note to my teacher explaining why my prework is late.
3. Email the note from my Gmail to hello@schoolrunbook.com.

## Details you'll need

- My sheet: [paste link]. Row 1 has the headers Animal, Adjective, School supply and Body of water. Row 2 has my words.
- Write the note yourself: three or four sentences, very formal and over the top, with a blank for each header. The note's wording stays the same; only the blanks change.
- Email subject: "Why my prework is late, from [your name]".

## Scope: keep it small

- Run it manually with a button. No schedule.
- Read one row only.
- No AI in the workflow.
- Use the fewest nodes that do the job.
```

<ol start="2">
  <li>Claude creates your guide with a Context tab and asks you any questions it has. Answer them.</li>
  <li>Claude gives you a line with your guide's link. Open your project's instructions, replace <code>[Links to be added]</code> with that line, and save.</li>
  <li>Read the Context tab. Edit it yourself or ask Claude to change anything that's missing or wrong. When it looks right, tell Claude to move on.</li>
  <li>Claude adds a Design tab. Read it, ask Claude about anything that's unclear, and edit it the same way. When the design looks right, tell Claude you're ready to build, and it adds the Build tab.</li>
</ol>

### Build it

1. In the SchoolRunbook n8n workspace, create a new workflow called `Late homework excuse - [your name]`.
2. Follow the Build tab one milestone at a time.
3. Tell Claude when you're ready for the next milestone.
4. On the last milestone, click **Execute workflow**. Your note goes to hello@schoolrunbook.com.

**Stuck?** Go back to the same Claude chat, describe where you are, and paste the error message or a screenshot. If you come back later, start a new chat in the project and paste your guide's link; Claude will pick up where you left off.

**Done when:** your guide has Context, Design and Build tabs with every milestone ticked, it's linked in your project instructions, and your note is in your Gmail Sent folder.

### Bonus: let AI write the excuse (optional)

Once your note arrives, try having AI write a fresh excuse every time. Our n8n workspace already has a Claude credential, so there's nothing new to set up. This is a preview of the AI step you'll build for homework after Class 1.

**Demo video:** coming soon

1. In the same chat, send Claude this:

```text
Let's add an AI step. Instead of the fixed note, have Claude write a longer, more dramatic excuse from my words each time the workflow runs. Use the Claude credential that's already in our n8n workspace. Update the Design tab, then add the new milestone to the Build tab.
```

<ol start="2">
  <li>Read the updated Design tab, then build the new milestone the same way as the others.</li>
  <li>Run the workflow two or three times. Each excuse should be different.</li>
</ol>

## 5. Prepare for the first class

**Why:** during the first class, we'll work on building an automation that processes emails sent to a financial inbox. Shortly before the class, you'll receive approximately 20 emails from "admin@schoolrunbook.com" that include sample invoices, reminders, etc. Please set up the filter below. It will ensure the emails don't go to Spam, stay out of your primary inbox, and have the label the automation needs to process them.

**Demo video:** coming soon

Use Gmail on a computer for these steps; the phone app can't create filters. Sign in with the same Google account you'll use for the course.

1. Click the **Show search options** icon at the right end of the Gmail search bar.
2. In **From**, type `admin@schoolrunbook.com`, then click **Create filter**.
3. Tick these three boxes:
    - **Skip the Inbox (Archive it)**
    - **Apply the label:** open the dropdown, choose **New label**, name it `srb-test` exactly as written (lowercase, with the hyphen), and click **Create**
    - **Never send it to Spam**
4. Click **Create filter**.

The label name matters: the automation only reads emails labeled `srb-test`, so a different spelling means it finds nothing. When the emails arrive they won't appear in your inbox. To see them, click `srb-test` in Gmail's left sidebar (it may be under **More**).

**Done when:** `srb-test` shows in your Gmail sidebar, and the filter is listed under Settings, See all settings, Filters and Blocked Addresses.
