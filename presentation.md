---
marp: true
theme: uncover
class: invert
size: 16:9
style: |
    section {
        text-align: left
    }

---
## Files and Folders **Migration Plan**
*6th Oct 2023*

---
## Why do we need to migrate to **Network Attached Storage (NAS)**
* It is a LEARN requirement
    * Local Storage
    * Cloud Storage

---
## NAS and Google Drive Comparison
<style scoped>section { font-size: 20px; text-align:left;}</style>
|Feature|Google Drive|NAS|
|--|--|--|
|Cost|Flexible Plan - 7.2 USD/user/month<br /> * Add or remove users anytime<br /><br />Annual plan - 6 USD/user/month<br />* Can add users anytime<br />* Cannot remove users after making payment|Initial Setup<br/>* No monthly/annual fees|
|Storage|30GB/user|Depends on HDD range from 2TB-30TB|
|Security|Data encrypted by Google but Google can view and scan the files|Data encrypted by own configuration|
|Accessibility|Anywhere online *(browser or explorer)*|Explorer on same network<br/>Browser on outside network|
|Performance|Data transfer speed depends on internet connection and Google's server load|Depends on own network speed and NAS performance|

---
## Whether NAS or Google Drive is primarily used, scheduled back up can be performed **bidirectional** between NAS and Google Drive.

---
## Data Flow Diagram (NAS)
### (2) Channels
1. Synology Client (Windows Explorer/ Mac Finder)
2. Synology Quickconnect (Web browser)

---
<style scoped>section { text-align:center;}</style>
![width:1000px](/assets/images/01.png)

---
<style scoped>section { text-align:center;}</style>
![width:1000px](/assets/images/02.png)

---
### Steps for migration from Google Drive to Synology NAS
* Directory Structure Setup
* Authentication and Authorization
* Migrating one department at at a time
* Move departmental folder from Google Drive to NAS *(the departmental folder will be deleted from Google Drive)*
* Install Synology client on departmental employee computers
* Login and create sync folders

---
### Directory Structure of NAS

<div style="position: relative; width: 100%; height: 0; padding-top: 100.0000%;
 padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
 border-radius: 8px; will-change: transform;">
  <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
    src="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAFn6i3DTpQ&#x2F;view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
  </iframe>
</div>
<a href="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAFn6i3DTpQ&#x2F;view?utm_content=DAFn6i3DTpQ&amp;utm_campaign=designshare&amp;utm_medium=embeds&amp;utm_source=link" target="_blank" rel="noopener">File &amp; Folder Structure for EHSSG</a> by EHSS Group

---
## Estimated migration time for each department ~ **1 day**
Directory migration usually takes only a few minutes.
Client setup and log in process may take longer than expected.

---
## Note: External viewers will **lose access**.
## You need to start **sharing the files and folders** again.

---
## **Google Sheet**, **Google Doc**, **Google Slide** will automatically converted to **Microsoft Excel**, **Microsoft Word**, **Microsoft Powerpoint**.

---
## Formulae and formattiing previously working perfect in Google Sheet may **misbehave** in Excel.

---
## If you are outside of the network *(home)*, you can still **edit** a file.
## It will **sync automatically** when you are reconnected to office network.

---
## If two persons edit the same file at the same time in Excel, Word, Powerpoint, when hit save, **2 files** will be saved separately, **even in the same office network**.

---
## If two persons edited the same file at home and get synced in office network, **2 files** will be saved separately.

---
## That kind of file conflicts will not occur in **QuickConnect**.
## What if we always use **QuickConnect**?

---
* QuickConnect always opens the files and folders through browser.
* Microsoft Office files can be opened with **Synology Office** in QuickConnect.
* **More than one person** can edit and save the same file in QuickConnect.
* QuickConnect works the same both on office network and outside.
* Formulae and formatting working perfect in Microsoft Office may **misbehave** in Synology Office.

---
<!-- _backgroundColor: white -->
<!-- _color: black -->
## Departmental Sequence
[![](https://mermaid.ink/img/pako:eNpV0L1uwyAUBeBXQXfolKi7h0iJ_6tGauNIHSDDlcExqgGLgqooyruXYNQ2TNzvXBjOFXrDBWQwTOa7H9E68npgmoSzpe3xRNbrDdnRPXki5Sl5tJy-WXO2qB60oLVF7ZLtopW08_M8XUg-otQpypdoGYr_QxmHijaH5y1Xvw-qyDWtpEbdi6R11IYebfha6vMDt_S9TdBEeKFl03U1-TD282-5XTJYgRJWoeShjes9YuBGoQSDLFy5GNBPjgHTt7CK3pnuonvInPViBX7m6EQh8V4JZANOX0EFl87Y_dJwLPr2A0E0afs?type=png)](https://mermaid.live/edit#pako:eNpV0L1uwyAUBeBXQXfolKi7h0iJ_6tGauNIHSDDlcExqgGLgqooyruXYNQ2TNzvXBjOFXrDBWQwTOa7H9E68npgmoSzpe3xRNbrDdnRPXki5Sl5tJy-WXO2qB60oLVF7ZLtopW08_M8XUg-otQpypdoGYr_QxmHijaH5y1Xvw-qyDWtpEbdi6R11IYebfha6vMDt_S9TdBEeKFl03U1-TD282-5XTJYgRJWoeShjes9YuBGoQSDLFy5GNBPjgHTt7CK3pnuonvInPViBX7m6EQh8V4JZANOX0EFl87Y_dJwLPr2A0E0afs)

---
<!-- _backgroundColor: white -->
<!-- _color: black -->
## Data migration timeline
[![width:1200px](https://mermaid.ink/img/pako:eNqF0k1Pg0AQBuC_stmDJ4hAq1VuRvrhgUSliTHhMrLTdiPsNtvh0DT97w6lpVWaOCey7zPsZnd2srAKZSyXYIhyI7hIU4kiAQKR6qUD0ta0iQLCiXUVkBBJ4qep_8nVZhssGvi3Jb0Zi3PFEHoiGPlh4EdBNPBEpFr26iy3VY2Iroup4xNyPLgeZ_V6XW7F8wq0YbUgdOJgH882PNrZ--2Tqi7ckLOg7ybagCmwY3cchX02d7ynNsvO3XMW9d3by39iPMuyqfiw7pt_F4sjHjEY9PHpwufO1l8lblbWEredzvRrsdv4gfuHl7cnPVkhv6hWPAS7pjmXtMIKcxnzp8IF1CXlMjd7plCTzbamkDG5Gj1Zr5uRSDQ0jyfjBZQbXkWlybq0HazDfO1_ALvjr2w?type=png)](https://mermaid.live/edit#pako:eNqF0k1Pg0AQBuC_stmDJ4hAq1VuRvrhgUSliTHhMrLTdiPsNtvh0DT97w6lpVWaOCey7zPsZnd2srAKZSyXYIhyI7hIU4kiAQKR6qUD0ta0iQLCiXUVkBBJ4qep_8nVZhssGvi3Jb0Zi3PFEHoiGPlh4EdBNPBEpFr26iy3VY2Iroup4xNyPLgeZ_V6XW7F8wq0YbUgdOJgH882PNrZ--2Tqi7ckLOg7ybagCmwY3cchX02d7ynNsvO3XMW9d3by39iPMuyqfiw7pt_F4sjHjEY9PHpwufO1l8lblbWEredzvRrsdv4gfuHl7cnPVkhv6hWPAS7pjmXtMIKcxnzp8IF1CXlMjd7plCTzbamkDG5Gj1Zr5uRSDQ0jyfjBZQbXkWlybq0HazDfO1_ALvjr2w)

---
<style scoped>
  section {
    text-align:center;
  }
</style>
# **Q  & A**