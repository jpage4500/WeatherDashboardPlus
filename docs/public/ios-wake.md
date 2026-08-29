**Automated iPad Deployment Guide**

Configuring iOS Devices to Auto-Wake and Launch Your App Every Morning

**Overview:** Apple iOS enforces strict sandboxing rules that prevent apps from waking a screen natively via

software. To achieve a hands-free morning wake cycle for your app, you must leverage hardware power

transitions combined with built-in Apple Shortcuts. This guide covers the **Smart Plug Power-Cycle**

**Method** and critical **Guided Access** optimizations to lock your app on screen.

**1. Hardware & System Prerequisites**

• **Smart Power Switch:** Any HomeKit, Home Assistant, Alexa, or standalone smart plug scheduled to cut

power briefly and turn back on every morning.

• **Power Adapter:** The iPad must remain physically connected to this smart plug via its charging cable.

• **Passcode Removal (Required):** Navigate to *Settings > Face ID & Passcode* and completely disable

the device passcode. If a passcode is active, the screen will wake to a lock screen but will block your

automation from launching the app.

• **Apple Shortcuts App:** Ensure the native Apple Shortcuts app is installed on the iPad.

**2. iPad Settings Optimization**

To ensure the iPad stays awake indefinitely after launching your app, configure the following settings:

• **Disable Auto-Lock:** Go to *Settings > Display & Brightness > Auto-Lock* and set it to **Never**.

• **Guided Access (Recommended Alternative):** If you prefer to allow standard iOS auto-lock when the

app is idle but want a bulletproof way to lock the user into your app, turn on Guided Access under

*Settings > Accessibility > Guided Access*.

**3. Step-by-Step Configuration Flow**

**Step A: Configure the Smart Plug Schedule**

Using your smart plug's native app (e.g., Apple Home, SmartLife, Home Assistant), set a daily recurring

morning rule:

1. **Time:** Choose your desired wake time (e.g., 6:55 AM).

2. **Action 1:** Turn the Smart Plug **OFF**.

3. **Action 2:** Turn the Smart Plug **ON** exactly 5 minutes later (e.g., 7:00 AM). The physical reintroduction

of power forces the iPad screen to instantly light up.**Step B: Build the Apple Shortcuts Automation**

On the deployment iPad, build a localized macro that intercepts the power event:

1. Launch the **Shortcuts App** and tap the center **Automation** tab.

2. Tap the **+** icon (or 'Create Personal Automation') to create a new macro.

3. Scroll down the list of triggers and select **Charger**.

4. Check the box for **Is Connected** and choose **Run Immediately** (do not select 'Ask Before Running').

Tap Next.

5. Tap **New Blank Automation**, then select **Add Action**.

6. Search for the **Open App** action, tap it, and click the blue 'App' placeholder to select your app from the

list.

7. Verify that 'Notify When Run' is disabled to ensure a seamless, quiet launch. Tap Done.
