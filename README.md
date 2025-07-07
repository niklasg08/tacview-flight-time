# Tacview Flight Time
Tacview Addon for Flight Time Measurement

# Origin
This Tacview Addon is initially from Buzybee. I modified it to fit it into my requirements.
When you want to use the original Addon, please go to: https://github.com/RaiaSoftwareInc/tacview.add-ons.lua
Basically, he only computed the life time of the primary and secondary object, which is not that accurate.

# Installation
First, download the `display-flight-time` zip-directory and unzip it to any directory.
Copy or Cut the `display-flight-time` folder to your `AddOns` folder in your root tacview directory.

Example path: 
```md
C:\Program Files (x86)\Tacview\AddOns
```

# Setup
1. In order to enable the addon, you maybe need to restart tacview after the installation.
2. Afterwards, click on the addon menu (gear icon).
3. Now, you can go to `Enable/Disable AddOns` and search for `Display Flight Time` and enable it with a click on it.

# Guide
The addon is straightforward. You can record an unlimited number of "flights".

To display the flight time for either your **primary** or **secondary** object:

1. Open the addon menu again (gear icon).  
2. Click on the `Flight Time` submenu.  
3. From there, select either:
   - `Set Primary Flight Time`, or  
   - `Set Secondary Flight Time`.

Each time you click, the current time is saved to a list. On every render frame in Tacview, the addon calculates total flight time using these time entries in **pairs**.

## What does that mean?  
- Entry `1` and `2` form a **pair** — representing one flight.  
- You can create multiple flights this way.  
- Each time you set a time, it either acts as a **takeoff** or **landing** time.  
- When a takeoff time is set, the addon uses the current time in the track to calculate the duration of the flight.

## Resetting Flight Time  
To reset a objects flight time:

- Go to the addon menu and click `Reset Flight Time` for the desired object.
