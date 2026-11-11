---
layout: default
title: GPSS/CK Support
---

# GPSS/CK

GPSS/CK is a Mac app for discrete-event simulation. You describe a system as a GPSS model — arrivals, queues, servers, storages and routing — run it, and study waiting times, utilization and throughput in reports, plots, an animation of the run and a debugger that can step back. The app includes the book *Queues, Clocks, and Choices: Discrete-Event Simulation with GPSS/CK* with all of its example models, a language reference, and the command-line tool `cksim`.

GPSS/CK runs on macOS 15 Sequoia or later, on a Mac with Apple silicon.

## Support

If you need help, please send an email to:

- [christian.klukas@gmail.com](mailto:christian.klukas@gmail.com)

In your email, please include:

- Your Mac model and macOS version
- The GPSS/CK version, shown under **GPSS/CK > About GPSS/CK**
- Your edition: Free, Personal or Professional
- What you were doing, and the steps to reproduce the problem
- What you expected and what happened
- The model file, or the smallest model that shows the problem, if you can share it
- For a problem with `cksim`: the command you ran, its output, and which terminal app you use
- A screenshot, if relevant

## FAQ

### Where do I start?

Choose **Help > Book Examples…**, select a chapter, and open an example. **Model > Check Model** validates it and **Model > Run Model** runs it. The tabs below the editor show the model diagram, the results, studies, the animation and the debugger. Each example names the page of the book that explains it.

### Where is the documentation?

All of it is in the app and works offline. **Help > GPSS/CK Help** explains the app, the **Reference** describes the language and the command line, and the book opens from the Help menu.

### What do the editions include?

| Edition | Models you can run | Optimization |
|---|---|---|
| Free | up to 150 blocks | not included |
| Personal | up to 1,500 blocks | included |
| Professional | any size | included |

Every edition can open, edit, check, draw and save a model of any size; the limit applies when a run starts. Personal and Professional are one-time purchases, and Professional requires Personal. There is no subscription and no account.

### How are blocks counted?

The limit counts the static size of the prepared model. Each block counts once, including blocks produced by repetition and by library expansion. Transactions, loops at run time, replications and simulated time add nothing. The **Help** tab shows the count of the open model under **Static model size**.

### I bought an edition but the app still shows the old one.

Open **GPSS/CK > Editions and Upgrades** and choose **Restore Purchases**. Make sure you are signed in to the App Store with the Apple Account that made the purchase. A pending or cancelled purchase does not unlock an edition.

### What is my GPSS/CK folder?

It is one ordinary folder that you choose once, for example a new folder named `GPSS-CK` in Documents. The book examples are installed there, and both the app and `cksim` may read and write in it. **Help > Show GPSS/CK Folder in Finder** opens it.

### How do I use GPSS/CK from Terminal?

Choose **Help > Use GPSS/CK from Terminal…**. The sheet shows one line to add to your shell profile so that the shell finds `cksim`, and the `cd` line for each folder `cksim` may use. Open a new Terminal window afterwards.

### cksim says a file is outside the registered folders.

macOS runs GPSS/CK and `cksim` in the App Sandbox, so `cksim` works only in folders you have registered for it. Register a folder once, either with **Add Folder…** in **Help > Use GPSS/CK from Terminal…** or with `cksim folders add <folder>`, which opens the system's folder dialog. `cksim folders` lists the registered folders.

### How do I withdraw a folder again?

Select it in **Help > Use GPSS/CK from Terminal…** and choose **Remove**, or use `cksim folders remove <folder>`. **Remove All…** and `cksim folders remove --all` withdraw every folder. No file is deleted; only the permission is withdrawn, for both the app and `cksim`.

### Terminal reports "Operation not permitted" in my Documents folder.

The first time a terminal app uses the Documents folder, macOS asks for permission. If it was declined, allow it under **System Settings > Privacy & Security > Files and Folders** for your terminal app.

### cksim runs with the Free limits although I own Personal.

`cksim` follows the edition of the app. After a purchase, open GPSS/CK once so the tool learns of it.

### Can I open models written for GPSS/H or IBM GPSS/360?

GPSS/CK has its own dialect and separate strict profiles for GPSS/H and IBM GPSS/360 source. A statement outside the selected profile is reported with its line rather than guessed at. The Reference lists what each profile accepts and where behaviour differs.

### May I use the book's example models in my own work?

Yes. The example models, their data files and the accompanying helper scripts may be used, copied, modified and distributed by anyone, for any purpose, without conditions and without attribution (CC0 1.0). This does not extend to the text and illustrations of the book.

## Privacy

See the [Privacy Policy](./privacy.html).

## Trademarks

GPSS/CK is an independent product. It is not affiliated with, endorsed by or derived from the products of IBM or Wolverine Software. IBM is a trademark of International Business Machines Corporation; GPSS/H is a product of Wolverine Software Corporation. These names are used only to say which model source GPSS/CK can read.
