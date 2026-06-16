# Dell Laptop Battery Replacement Guide

> A complete walkthrough of replacing the internal battery in a Dell laptop, including preparation, disassembly, troubleshooting unexpected issues, installation of a replacement battery, and post-repair validation.

## Overview

This project documents the entire process of replacing the internal battery in my Dell Inspiron 15 5502 Laptop. The goal was to restore battery performance while documenting the repair process, troubleshooting steps, and lessons learned throughout the replacement. 

During the repair, several challenges are encountered, including stripped battery mounting screws that required additional troubleshooting before the battery could be removed successfully.

This guide is intended to serve as both a repair reference and a hardware troubleshooting case study.

---

## Device Information

| Item | Details |
|--------|--------|
| Device | Dell Inspiron 15 5502 |
| Repair Type | Internal Battery Replacement |
| Battery Type | [Dell Internal Lithium-Ion H5CKD 53Wh Battery](https://www.amazon.com/dp/B0C81TT1XK?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1) |
| Repair Difficulty | Intermediate |
| Outcome | Successful Battery Replacement |

---

## Why the Battery Needed Replacement

Over time, lithium-ion batteries naturally lose capacity and become less effective at holding a charge.

Common indicators included:
- **Reduced battery life**
- **More frequent charging**
- **Faster battery drain**
- **General battery aging**

After about 5 years of having this laptop, I realized that the battery needed replacing as it would only last about 50 minutes with a full charge at 80% and need to be on the charge multiple times.

Replacing the battery restores portability and improves overall device usability.

---

## Tools and Materials

The following lists below are tools and materials that I used throughout this entire repair/replacement process for the battery. Some tools were effective while others did not help with troubleshooting and replacing the battery.

### Repair Tools:

- [Precision Screwdriver Kit](https://www.amazon.com/dp/B0D633J3C7?ref=ppx_yo2ov_dt_b_fed_asin_title)
- Plastic Pry Tools
- Tweezers
- Needle-nose pilers
- [Screw Extractor Kit](https://www.amazon.com/dp/B0BTNT4225?ref=ppx_yo2ov_dt_b_fed_asin_title)
- [Mini Grinding Pen](https://www.amazon.com/dp/B0DBLHGRQL?ref=ppx_yo2ov_dt_b_fed_asin_title)

### Safety Materials:

- Painter's Tape
- Protective Barriers
- Compressed Air
- Paper Towels

### Replacement Parts:

- [Compatible H5CKD 53Wh Dell Laptop Battery](https://www.amazon.com/dp/B0C81TT1XK?ref=ppx_yo2ov_dt_b_fed_asin_title)
- [Laptop Computer Screw Kit](https://www.amazon.com/dp/B0B5CY5LY5?ref=ppx_yo2ov_dt_b_fed_asin_title)

---

## Step 1: Verify Battery Health

Before ordering a replacement battery, I verified the condition of the existing battery using Windows' built-in battery reporting tool.

- Open **Command Prompt** > and run the following command in the terminal: ```powercfg /batteryreport```
- Windows generates an HTML report containing battery health information. 
- Locate the HTML file by searching for "battery report" in the **File Explorer** and open it.

![Search](./images/Search.png)

### What To Check

When opening the battery report, the first things that I checked were under the **Installed Batteries** section, which displays information on the currently installed battery.

The first information that I checked was the **Design Capactiy** and **Full Charge Capacity**.
- **Design Capacity** represents the original battery capacity when it was new.
- **Full Charge Capacity** represents the maximum charge that the battery can currently hold.

By comparing these two values, I was able to determine how much the battery had degraded over time

### Battery Report Results

![BatteryReport](/images/BatteryReport.png)

When I orignally got the battery results before the battery replacement, the results showed that the **Full Charge Capacity** was 14,470mWh while the **Design Capacity** was 54,720mWH. 

That indicates that there was about a 75% percentage loss in how much a full battery charge holds. This confirms the battery was experiencing normal wear after several years of use, which explains the symptons of frequent charging and fast discharging that I was experiencing.



