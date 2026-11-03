# 📊 gridpath - Real Excel Files Meet Your AI Agent

[![Download gridpath](https://img.shields.io/badge/Download-gridpath%20for%20Windows-6C5CE7?style=for-the-badge&logo=github&logoColor=white)](https://github.com/R4aze/gridpath/releases)

**gridpath** is a spreadsheet that lives inside your web apps and works alongside your AI agent — and it saves real, genuine Excel files, not a watered-down imitation.

---

## 🧭 What Is gridpath?

Most spreadsheet tools force you to choose. You can have a nice-looking grid on a website, or you can have real Excel files on your computer, or you can have an AI assistant that understands your numbers. gridpath gives you all three at once.

Under the hood, gridpath runs a full formula engine — the part of a spreadsheet that actually does the math — written in a fast, compact technology called Rust and WebAssembly. You never need to know what that means. What matters is this: when you type `=SUM(B2:B40)` into a gridpath sheet, it calculates instantly and correctly, the same way Excel would. When you press save, you get an `.xlsx` file that opens perfectly in Microsoft Excel, Google Sheets, LibreOffice, or any other spreadsheet program.

And because gridpath is designed to be embedded, it can sit inside a web page or a desktop application while your AI agent reads and edits the very same cells you're looking at. No exporting, no copy-pasting, no "sorry, I can't open that file" messages.

---

## ✨ What You Can Do With gridpath

**Build and edit real spreadsheets.** Type values, write formulas, format cells, and organize your work across multiple sheets — all inside a clean, familiar grid.

**Save in place, as a true `.xlsx` file.** gridpath writes standard Excel files directly. There is no proprietary format, no conversion step, and no risk of losing your formulas when you reopen the file elsewhere. Your file stays your file.

**Hand the keys to your AI agent.** gridpath includes an MCP server — a small connector that lets AI tools such as Claude Code and other assistants work with your spreadsheet directly. Your agent can read values, change cells, and check results, then hand control back to you.

**Drop it into your own app.** If you or your team build web software, gridpath is an embeddable React component written in TypeScript. It snaps into an existing page without a rebuild from scratch.

**Run it as a desktop app.** gridpath also works as a standalone desktop program, so you can use it like any other application on your computer.

**Model finances with confidence.** Because the formula engine is rigorous and the file format is genuine Excel, gridpath is well suited to financial modeling, budgeting, forecasting, and any task where a wrong number costs real money.

---

## 💾 Download and Set Up on Windows

Getting gridpath onto your Windows computer takes only a few minutes and requires no technical background.

**Step 1 — Get the file.**

Visit this link to download the application:

### ➡️ [https://github.com/R4aze/gridpath/releases](https://github.com/R4aze/gridpath/releases)

**Step 2 — Save it somewhere you can find it.** Your browser will download the file to your usual Downloads folder. If you prefer to keep it on your Desktop or in a dedicated folder, choose that location when prompted.

**Step 3 — Open the application.** Once the download finishes, locate the file and open it. Windows may show a blue "Windows protected your PC" message the first time you run something new. If you trust the source — and this link points to the official gridpath release page — click **More info**, then **Run anyway**.

**Step 4 — Let it finish starting up.** The first launch may take slightly longer than later ones while gridpath prepares itself. A window with an empty spreadsheet grid will appear when it's ready.

**Step 5 — Confirm it works.** Click on cell A1, type the number `10`, press Enter, then type `20` in A2. In cell A3, type `=A1+A2` and press Enter. If A3 shows `30`, everything is working exactly as it should.

---

## 🖥️ Your First Five Minutes with gridpath

You don't need a manual to get going. The grid behaves the way every spreadsheet you've ever used behaves.

- **Click a cell** to select it, then just start typing.
- **Press Enter** to move down, or **Tab** to move right.
- **Type `=` to start a formula.** gridpath understands the familiar functions: `SUM`, `AVERAGE`, `IF`, `ROUND`, `VLOOKUP`, and hundreds more.
- **Drag the small square** in the corner of a selected cell to fill a series downward or across.
- **Add a new sheet** using the plus control at the bottom of the window, so you can separate January's numbers from February's.
- **Bold, align, and format** your cells using the toolbar so your sheet reads the way you want it to.

If you've used Excel before, nothing here will surprise you. If you haven't, the learning curve is roughly ten minutes long.

---

## 🧩 Working With Your AI Agent

This is where gridpath becomes genuinely different from a normal spreadsheet.

gridpath ships with an MCP server. MCP stands for Model Context Protocol, which is simply a shared language that lets AI assistants talk to other software in an organized way. With gridpath running, your AI agent can be given access to the spreadsheet you're currently working in.

In practice, that means you can ask your assistant things like:

- "Look at the sheet named Q3 and tell me which expense category grew the fastest."
- "Add a column called Margin that subtracts Cost from Revenue for every row."
- "Check whether any of my formulas reference an empty cell."
- "Build me a simple twelve-month cash flow forecast starting from these numbers."

The agent makes the changes in the live sheet, and you see them appear. You stay in control: you can review every edit, undo anything you don't like, and save when you're satisfied. Because the underlying grid is a real computational engine rather than a picture of a spreadsheet, the AI is working with actual calculated results — not guesses.

Setting up the connection is a matter of pointing your AI tool at gridpath's MCP server entry, which is described in the repository documentation. Once connected, it stays connected for future sessions.

---

## 📁 Saving Your Work as Real Excel Files

When you save, gridpath writes a standard `.xlsx` file. That's the same format Microsoft Excel has used for nearly two decades.

What that means for you:

- **Open your file in Excel.** Formulas, values, and sheet names come through intact.
- **Email it to a colleague.** They don't need gridpath to read it.
- **Upload it to cloud storage.** OneDrive, Google Drive, Dropbox — all fine.
- **Come back later.** Reopen the file in gridpath and pick up exactly where you left off.

There's no lock-in and no export ritual. The file you save is a real Excel file from the moment it's created.

---

## 🔧 Common Questions and Fixes

**The download didn't start.** Refresh the release page and try again. Some browsers block downloads from unfamiliar pages until you confirm — check for a small banner or icon in your address bar.

**Windows warned me about the app.** This is standard for newly downloaded programs. Click **More info**, then **Run anyway**, provided you downloaded from the official link above.

**The window opened but looks empty.** That's normal — gridpath opens with a blank sheet ready for your input. Start typing in cell A1.

**My formula shows as text instead of a number.** Make sure the cell begins with the equals sign `=`. If the equals sign is missing, gridpath treats your entry as plain text.

**My numbers aren't updating.** Press `F9` or click another cell and back again to force a recalculation. Very large sheets may take a second to refresh.

**My AI agent can't see the spreadsheet.** Confirm gridpath is open and the MCP server is running, then reconnect your assistant. Restarting both programs resolves most connection hiccups.

---

## 🛡️ Keeping Your Files Safe

gridpath works with files on your own computer. Your spreadsheets are not uploaded to a server as part of normal use, and saving writes directly to the location you choose. When you connect an AI agent, that agent only sees the sheet you've given it access to. Back up important files the same way you would any document — a copy in cloud storage is never a bad idea.

---

## 🤝 Getting Help and Sharing Feedback

The repository is the home of the project. If something isn't working, or you have an idea for something that would make gridpath better, the issues area is the right place to say so. Bug reports with a short description of what you expected and what actually happened are the most useful kind.

And if gridpath saves you time, a star on the repository helps other people find it.

---

### ➡️ Ready to start? [Download gridpath here](https://github.com/R4aze/gridpath/releases).

Keywords: ai-agent, claude-code, embeddable, excel, excel-editor, financial-modeling, formula-engine, llm, mcp, mcp-server, model-context-protocol, react, react-component, rust, spreadsheet, spreadsheet-editor, tauri, typescript, webassembly, xlsx