

# Work offline as an operator in Dynamics 365 Guides

You can work offline with a guide on HoloLens 1 or HoloLens 2 (for example, if you're on a field service call or working on a factory floor) if you don't have access to the internet or have an intermittent internet connection. 

You don't need to do anything to set up **Offline** mode. When you open a guide when you're connected to the internet, the guide is automatically downloaded for offline use. If you lose your internet connection or turn off your Wi-Fi connection, the guide will automatically be available and you'll see the **Offline** banner at the top of your screen.

![Offline mode](media/offline-mode.PNG "Offline mode")

Any guide that's available for offline use will appear under the **All** tab. If no guides are available offline, you'll see this message: 

"No guides are available offline."

## Signing in while offline

If you go offline, Dynamics 365 Guides automatically signs you into the last account you used when you were online. 

> [!IMPORTANT]
> If you sign out when you're offline, you won't be able to sign back in again until you reconnect to the internet.

## Working with multiple users or devices

Guides are specific to the user and the HoloLens. If you're sharing a HoloLens with another user and you both want to use the same guide, each of you will need to open the guide when you have an internet connection to automatically download the guide. 

Likewise, if you use more than one HoloLens, you'll need to open the guide on each HoloLens while you have an internet connection so you can download the guide for offline use.

## Accessing a guide offline with a QR code

You can access a guide using a QR code link as long as you've used the guide while you had an internet connection.

## Using the Dynamics 365 Guides demo when you're offline

The demo available through the Dynamics 365 Guides Home screen is available for use without an internet connection.

## Limitations with Offline mode

- You can't author a guide in **Offline** mode.

- If you make changes to a guide as an author, those changes will not automatically apply to your downloaded guide. You must re-open the guide on the device you want to use offline to make sure the latest changes have been dowloaded. When you're offline, the guide will show the date that iw as last downloaded to your device. If this date is before your most recent changes, the guide is out of date. Open it online to download the latest changes.

- If a guide is deactivated after it's downloaded to a device, the downloaded version will remain on the device until the cache is cleared, but users will not be able to access any updates or open it online.

- If you lose permissions to a guide that has already been downloaded to your HoloLens, the downloaded version will remain on the HoloLens until the cache is cleared, but users will not be able to access any updates or open it online. 



