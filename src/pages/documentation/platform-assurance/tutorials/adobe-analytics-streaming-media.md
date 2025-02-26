# Adobe Analytics for Streaming Media view in Assurance

## Overview

With the integration between Streaming Media Analytics and Adobe Experience Platform Assurance, you can now validate the Media Analytics implementation in your mobile app. Media Analytics views display what is tracked in the media session, such as:

* Session start event that contains all content core, standard metadata, and custom metadata properties, as well as session end and session complete events.
* Ad Break Start and Ad Start events with all ad properties attached, as well as Skip and Complete events for both.
* Chapter Start with all properties attached, as well as Chapter Skip and Chapter Complete events.
* All playback change events (play, pause, buffer, errors, bitrate change).
* All player state change tracking events (start, end).

Once data is processed in Analytics, post-processed status and data, such as media time spent and total pause duration, are also available in the event detail view.

## Use Assurance with Adobe Analytics for Streaming Media

After you have connected and [set up](../set-up.md) your app for Adobe Analytics, you are ready to configure it for Streaming Media Analytics. At the bottom of the left panel, click **Configure** to add the Media Analytics Events view and **Save** it.

![Configure](./assets/adobe-analytics-streaming-media/configure.png)

Once added, select the **Adobe Analytics &gt; Media Analytics Events** view to validate your session tracking.

![Select](./assets/adobe-analytics-streaming-media/select.png)

In the Media Analytics Events view, you may search and filter by Session ID (VSID) to view a specific media session. To view additional event details, select a specific event.

![Media Events](./assets/adobe-analytics-streaming-media/media-events.png)

For a more succinct view of API calls, you may also hide the playhead update events by selecting the **Hide Playhead Update events** filter.

![Hide Playhead](./assets/adobe-analytics-streaming-media/hide-playhead.png)

<InlineAlert variant="info" slots="text"/>

Viewing post-processed media analytics data requires the use of SDK versions: Android Media 2.1.2 and iOS AEPMedia 3.0.1 (or above)

To view post-processed data, find the session start event and validate in the status column that the session was completed. If completed, click on the event to view a media session summary in the event detail view. For further details, scroll down to find the post-processed details.

![Post-Processed View](./assets/adobe-analytics-streaming-media/post-processed-view.png)
