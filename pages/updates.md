---
layout: page
title: Updates
---

# Updates

We will aim to update this weekly!

## 3-27-2024

Next couple weeks we're focusing on communications, the website, and organizing. This will include: scheduling a hack-a-thon, refining a slide deck for community training sessions, documenting alert and management workflows, finalizing a report form.

Here's some updates on SpikeAlerts_Mpls:

* Version1.0 is shut down
    * Alerts were archived
    * User data has been deleted across all platforms
* Version2.0 is in a "soft release" stage:
    * There will be bugs...
    * 5-10 new users are manually added Mondays - capping at 150
    * We're committed to keep it running through this summer
    * There's a new, experimental report option on the [Realtime webmap](https://www.mplsaqalert.com/map/) and [Coverage webmap](https://www.mplsaqalert.com/map/coverage) (We're going to publish the webmap code in April)
    * The dataset ([Google Drive Link](https://drive.google.com/drive/folders/1u0hirGJlINDi_Ych8aH5ocUGfqtt2SID?usp=drive_link)) has changed slightly (We think for the better! More on this soon)
    
**Final note:** It has come to our attention that the lower PurpleAir PM2.5 Values (<50ug/m^3) used in our current system may be slightly over-estimated (not converted into US EPA/not accounting for humidity - [more here](https://community.purpleair.com/t/is-there-a-field-that-returns-data-with-us-epa-pm2-5-conversion-formula-applied/4593)). This is going to be a priority to investigate for Version2.1

## 3-22-2024

More in-depth update coming soon - been taking a little breather here.

We've had really good air quality this week so no alerts have been sent, yet. The first 10 sign-ups were added to the system this past Monday and everything appears to be running smooth! Writing the first report for version 2.0 and adding more folks this upcoming Monday.

## 3-15-2024

SpikeAlerts2.0 (v2) has been running most of this week without a hitch! 

We've messaged folks from Version 1.0 (v1) that we'll quietly shut down that service Sunday night and included the [sign-up form](https://redcap.ahc.umn.edu/redcap/surveys/?s=NH7JNNNR8LNCT8CN) for Version 2.0. On Monday, we'll delete all user data from v1, archive the alerts, and import new users into v2.

Also, the Minneapolis-specific website is up! We're just working on content and formatting the pages. Super excited to have a [realtime webmap](https://www.mplsaqalert.com/map/) now!

## 3-8-2024

It's been an exciting week! 

The new website is coming together complete with our own webmaps (see a [snapshot](../figs/example_webmap.html)) while the "Users & Notifications" extension of SpikeAlerts has been tested. This extension was pulled into the [Minneapolis instance](https://github.com/SpikeAlerts/SpikeAlerts_Mpls) for implementing SMS Messaging and REDCap scripts. 

A new sign-up form should be finished today and sent out to a focus group. Trial run to begin next week!

## 2-29-2024

Apologies for the delay in writing an update. Last week battling illness, this week playing catch up.

[REDCap](https://ctsi.umn.edu/tools/redcap) is undergoing a big update this weekend, and we won't be able to look up any phone numbers. So no SpikeAlerts from Friday to Monday, unfortunately. We'll still be watching the sensors, though!

In other news, we're getting very close to testing the new version! The workflow to monitor the sensors, create/delete alerts, and  check "Places of Interest" has been tested and runs smooth. The last piece of the puzzle is the "Users & Notifications" extension of the project which is quickly falling into place. 

Next week we'll be intensively working on the new website and organizing a focus group to test the new version! 

## 2-14-2024

[Version 2.0](https://github.com/SpikeAlerts/SpikeAlerts) has the full workflow public on Github. A little more documentation/testing and development of the "Users & Notifications" extension then we will fork this and begin developing the Minneapolis instance of SpikeAlerts (SpikeAlerts_Mpls)! This is where we can start the work to include all of the user feedback we've received!

We noticed that our SpikeMovies were getting viewed/downloaded too much, and Google throttled our Drive. The workaround (for now) is having a [Youtube channel](https://www.youtube.com/@SpikeAlerts) for folks to view. Download links will be sent upon request.

Lastly, the lead developers discussed serving our own website for SpikeAlerts_Mpls complete with a webmap of the real-time information (and potentially a discussion board). This website will then transition into more of a landing page for the greater SpikeAlerts project. To begin early March.

## 2-7-2024

The base of [version 2.0](https://github.com/SpikeAlerts/SpikeAlerts) runs smooth (up to updating alerts). We've also made an informational brochure for distributing at community events, schools, etc.

Next week we'll start working on updating the website, adding the Places of Interest (POIs formerly "Sign Up Information") & Reports, and developing flask apps (API and webmap).

## 1-31-2024

Paused overnight alerts and removed "SpikeAlert" from all messages. Significant work on code organization/modulation ([Repository](https://github.com/SpikeAlerts/SpikeAlerts)) - the new version should be ready for testing late February. 


## 1-24-2024

Version 2.0 is in progress! In March we will message when it's ready with a new sign-up form and then terminate version 1.

Currently, we are working on: materials for outreach; organizing researcher/programmer collaboration; investigating other sensors to incorporate into the system; and getting feedback for development of SpikeAlerts2.0

So far, our priorities for this next version include:

- Improving the "user experience"
- Translating all messaging into Spanish
- Including more educational resources and project documentation on website
- Making data publicly available in real-time
- Ensuring that reports are directed to agencies in the most actionable and timely manner
- Improving git structure and code organization for collaboration with other cities
