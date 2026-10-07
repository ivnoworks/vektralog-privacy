# Vektralog Privacy Policy

**Effective date: 2026-10-08**

Vektralog is a ride logger for motorcycles, cars and bicycles, made by
Ivnoworks. It is built local-first. There is no Vektralog
account and no Ivnoworks server: nothing you record is ever sent to us,
because there is nowhere to send it.

## In short

- Your rides, garage, settings and the photos you add to a ride are stored
  on your phone.
- Vektralog has no analytics, no advertising and no tracking code of its own.
- Location is recorded only while a ride is recording, never outside one.
- Heart rate from your watch, where offered and only if you turn it on, is
  read from Health Connect when you open a ride and is never stored.
- Two things can leave by themselves. The Google map: while it is on
  screen, Google's Maps SDK sends Google its own usage data (you can switch
  to the MapLibre map in Settings). And the weather, on unless you turn it
  off in Settings > Weather: after each ride, two positions rounded to about
  11 km and the ride's hours, and while a ride records, the rounded square
  you are in and the hour, at the start and every half hour, go to
  Open-Meteo. Never the track.
- Everything else that leaves your phone is something you chose to send:
  an export, a shared image, an SOS text, a backup you turned on.

## What Vektralog stores on your phone

- **Rides:** GPS track points (position, altitude, speed, heading and their
  accuracy), what the phone's GPS receiver reported with each point (how many
  satellites it used and could see, how strong their signals were and which
  satellite systems they belong to), timings, and what is measured from
  them, with the phone's own
  battery charge and percentage at the start and end of each ride, so
  Settings can say what recording costs your phone. A recording starts
  only when you press Record, in the app or from its Quick Settings tile,
  or, if you turn auto-record on, when a Bluetooth device you chose
  connects.
- **Sensor readings during a ride:** the motion sensors for lean angle,
  g-forces and harsh braking or acceleration, and how much the road shook
  the phone between one GPS point and the next, kept with each point; the
  barometer for altitude,
  where the phone has one; and a short burst of accelerometer readings once
  a minute to warn you when a rigid mount is shaking the phone. None of
  these run while no ride is recording.
- **The ride's own log:** what the recorder noticed about itself during each
  ride, kept with the ride: when recording started and stopped and how (by
  you, by your chosen device, after a restart, or because Android stopped
  it), the phone's heat steps, your chosen device dropping and coming back
  (never its name or address), journal write errors with a short error
  message, the GPS positions the app refused and why, with how far and in
  which direction a refused position lay from the last accepted one (the
  refused position itself is not kept), where the lean angle's zero was
  taken, which app version, phone model, Android version and GPS chip
  recorded the ride, which motion sensors the phone has, whether its
  positions came from the fused provider or the GPS chip, whether a
  mock-location app was supplying positions, and when the app's own live
  check thought the GPS was disturbed and when it was clear again. It
  travels with the ride into your backups and into the data export.
- **GPS disturbance:** whether a ride's GPS looked disturbed (its signal
  falling with the sky open, positions jumping or refused from far away) is
  worked out on the phone from what is already kept with the ride, each
  time you open it. That reading itself is not stored and never leaves the
  phone.
- **Light sensor:** read and never stored, to switch the automatic theme
  between day and night.
- **Sunlight:** each ride's sunrise, sunset and dusk, the stretches ridden
  with a low sun ahead or behind, and the minutes ridden after sunset and
  in the dark are worked out on the phone from the ride's own positions and
  times, every time you open the ride. Nothing is looked up, sent or stored
  for them.
- **Roads you ride again:** when rides go from the same start to the same
  end along the same road, the phone keeps a simplified line of that road
  (where it starts and ends, and its shape) and each ride's time along it,
  so a ride can be compared with your earlier rides of it. It is worked out
  on the phone from the rides' own tracks and stays there: it is not in the
  backup folder or the Drive backup, not in any export, and not on the
  share card. Android's own backup copies the app's database whole, so it
  carries these lines as it already carries the tracks they were drawn from.
- **Weather (on unless you turn it off):** for each ride whose weather was
  looked up, the hourly weather Open-Meteo answered for its two rounded
  places, kept with the ride. The temperature shown while you ride is kept
  only in memory and never stored. See Weather below.
- **Ride photos:** a reduced copy of each photo you add to a ride from
  your gallery. See Ride photos below.
- **Garage:** the vehicles you add, their photos, fuel and service entries,
  notes, and the documents you keep in each vehicle's glovebox.
- **Crash detection:** if you set up Crash SOS, the impacts the detector
  considered and rejected in the last 30 days (when, how hard, and why it
  said no), so you can see what it is doing. No position is kept with them.
- **Settings,** and in the garage the Bluetooth address of the device you
  picked for each vehicle's auto-record, and your SOS contact's name and
  number. For auto-record
  it also keeps when you last opened your phone's autostart setting from
  the app, and when a chosen device last started the app while it was
  closed, so the auto-record screen can say the setup has worked. When
  the app ends a ride by itself it keeps which ride and why (its device
  disconnected) until that ride's summary has told you, then forgets it.
- **Heart rate:** nothing. See Heart rate from your watch below; the one
  thing kept is when this phone's Health Connect first let Vektralog read,
  so the app can explain Health Connect's 30-day limit.
- **Why the app last stopped:** when a ride was cut short, Android's own
  record of why the app closed is read on the phone to explain it. It is
  not stored or sent anywhere.

## What leaves your phone, and when

**The map.** Map tiles are downloaded while a map is on screen, including
the live map during a ride, so a tile server can tell which area is being
looked at. Your recorded track is drawn on the phone and is never sent.

- **Google map (the default):** Google's Maps SDK draws it. It sends Google
  the tile requests and, by Google's own disclosure, crash logs,
  diagnostics, a device identifier and map interactions, which Google uses
  to run and improve its services. See Google's
  [Maps SDK data disclosure](https://developers.google.com/maps/documentation/android-sdk/play-data-disclosure)
  and the [Google Privacy Policy](https://policies.google.com/privacy).
  On a phone without usable Google Play services, which Google's map
  cannot run without, the MapLibre map draws in its place.
- **MapLibre map:** tiles come from [OpenFreeMap](https://openfreemap.org),
  terrain shading from [VersaTiles](https://versatiles.org) and, only if
  you turn those layers on, CyclOSM and OpenTopoMap. Each request carries
  only the tile being viewed and the app's name, version and the contact
  address below, which the OpenStreetMap tile usage policy requires.
  Offline map regions you download come from the same servers.

**Things you send yourself.** Each happens only when you tap it, goes only
where you send it, and Vektralog keeps no record of where that was:

- exporting rides (GPX), all your data (a zip), or a car's mileage log (CSV).
  The zip carries each ride's own log (the list above) as ride-log.csv.
  The zip opens with a README that describes the files beside it and states
  four things about the export itself: the app version, when it was made,
  your phone's UTC offset at that moment, and the name of any part you
  chose to leave out, without saying how much of it there is. The zip
  carries no Bluetooth address: its vehicle list names the device that
  starts auto-record and leaves the device's address on the phone (your
  backups keep it, so a restore can find the device again);
- sharing a ride card image, which has no map and no date unless you add one;
- the SOS text: Vektralog opens your SMS app with the message and your last
  position already written, and **you press send**. Nothing is sent
  automatically;
- opening where one of your cars or motorcycles was parked (the last point
  that vehicle's own last ride logged before it was paused or stopped,
  already on your phone) in a maps app. Until you tap it, the spot stays on
  the phone: Home draws the road into it from the ride's own track, with no
  map tile and no place-name lookup;
- opening a stored document in a viewer app.

**Backups you turn on,** described under Backups below.

**The weather, unless you turn it off,** described under Weather below.

Ivnoworks receives none of it.

## Location

- **While using the app:** asked the first time you press Record, to record
  the ride you started.
- **All the time (optional, auto-record only):** asked only if you turn
  auto-record on, after a screen that explains why. Android requires it for
  a ride to start while the app is closed, when your helmet, car or other
  chosen device connects. Vektralog still records location only while a
  ride is recording. Turning auto-record off, or taking the permission away
  in Android's settings, ends it.

## Crash SOS

Optional, and off until you set it up. While a ride records, Vektralog
watches the accelerometer for an impact. If it judges one to be a crash, it
shows a countdown you can cancel. When the countdown ends it opens your SMS
app with a message to your chosen contact and a map link to your last
position, and you press send. On a bicycle, and on a phone whose motion
sensor cannot sense an impact, SOS is manual only: nothing watches the
accelerometer, and the countdown starts when you press the SOS button. Your
contact's name and number stay on this phone and are left out of every
backup.

## Voice (on unless you turn it off)

On unless you turn it off: Vektralog ships with it on, and Settings >
Voice turns it off. Before 8 October 2026 it was off until you turned it
on; an install that never opened Settings > Voice comes up on with that
day's version, and one that did keeps the choice it holds. It speaks only
while a ride records, and never otherwise. While a ride records,
Vektralog says short lines through a headset or a car's Bluetooth when
one is connected, and otherwise through the phone's own speaker (or not
at all, if you choose "Only through a headset or the car"): the
ride starting and saved, its distance, time and top speed, the GPS
dropping and coming back, the phone getting too hot, the crash SOS. The
words are spoken by Android's speech engine, a separate app on your phone
under its own privacy policy, with a voice installed on the phone that
works offline: Vektralog never chooses a voice that needs a connection, so
nothing it says is sent anywhere. To decide whether and where to speak it
reads only which kind of audio output the line would play on (Bluetooth,
wired, USB or the phone's speaker), whether a call is in progress, and
whether the media volume is at zero, so Settings > Voice can say why
nothing would be heard. It reads no device names or addresses and
does no Bluetooth scanning, and nothing spoken is stored.

## Weather (on unless you turn it off)

On unless you turn it off: Vektralog ships with it on, and Settings >
Weather says what is sent and turns it off. Before 3 October 2026 it was
off until you turned it on; an install whose rider never touched the
switch came up on with that day's version, and a rider who had turned it
off stays off. While it is on, Vektralog asks Open-Meteo (open-meteo.com) for
weather in two ways, each time naming only places rounded to one decimal
of a degree, about 11 km, never the track, the vehicle or anything that
names you; the request carries the app's name and no details of your
phone.

- **After a ride:** the hourly weather at two places, where the ride began
  and where it ended, for the hours the ride lasted. Asked from its summary
  or when you open it, and from Home for every ride that has none yet —
  the rides you recorded before included, filled in once, newest first, a
  few at a time (one request every two seconds, rides of the same day in
  one request, no more than 400 requests a day). Nothing about a finished
  ride is sent while a ride records.
- **While a ride records:** the temperature at the rounded square you are
  in, for the hour now, asked when the ride starts, then every half hour or
  when you enter another square, and never while the recording screen is
  off. The answer is shown on the recording screen and kept only in memory:
  it is not stored with the ride or anywhere else.
- **What Open-Meteo sees:** like any website, your internet (IP) address,
  and by its own terms it keeps its logs, which may include the request,
  for 90 days. Open-Meteo is a third party and does not work for Ivnoworks.
- **What is kept:** a ride's answer, the hourly weather for its two rounded
  places, is stored with the ride and goes into your backups; the data
  export (zip) does not carry it. The temperature, wind and rain a ride
  shows are worked out from it on the phone, with the ride's own altitude,
  which is never sent.
- **Stopping it:** turn it off in Settings > Weather and nothing more is
  sent, after a ride or during one; a ride already looked up keeps its
  answer. Deleting a ride deletes its weather.
- **A new phone:** the weather switch itself is left out of every backup,
  so an old phone's "on" never comes across. Only an "off" travels: if you
  turned weather off, Android's backup and device transfer carry that one
  setting, and a phone restored from them keeps weather off. A phone set up
  without them starts with weather on, as a new install does.
- Weather data by Open-Meteo.com, under the CC BY 4.0 licence.

## Heart rate from your watch (optional)

Offered only in some builds, off until you turn it on in Settings > Heart
rate, and only once you allow it in Health Connect, Android's own store of
health data. Your watch's app (Mi Fitness, for example) writes your heart
rate to Health Connect under its own privacy policy; Vektralog asks
Health Connect for one thing, permission to read heart rate, and nothing
else.

- **When it reads:** only while it is turned on, and only when you open a
  ride, its summary or its GPX export: the heart rate recorded during that
  ride's own time, plus two minutes before and one after, to see a rise
  after a hard brake. Settings > Heart rate reads only the newest reading
  of the last 30 days, to show when your watch last synced. It never reads
  in the background and never reads to fill a history.
- **Not stored:** the readings are held in memory while the app is open
  (the last few rides you opened) and are not stored on the phone, not
  sent anywhere and not in any backup. The one thing kept is when Health
  Connect first let Vektralog read, because Health Connect shares only the
  30 days before that moment; it stays on this phone and is left out of
  every backup.
- **Exports:** a ride's GPX file carries its heart rate only if you tick
  Include heart rate when you export it. The data export (zip) never does.
- **Stopping it:** turn it off in Settings > Heart rate, or take the
  permission away in Health Connect > App permissions > Vektralog; a ride
  opened after that shows no heart rate.

## Ride photos

You can add photos to a ride. Add photos opens **Android's own photo
picker**, and only the photos you choose there reach Vektralog: it has no
permission to read your photos and **never sees your gallery**. Of each
photo you choose it keeps a **reduced copy** (at most 1600 pixels on the
long side) inside its private storage on this phone, filed with that
ride; the original in your gallery is not changed, moved or uploaded.
Removing the photo, or the ride, removes the copy. Ride photos are
**left out of Android's cloud backup, the backup folder and the Google
Drive backup**, and the data export does not carry them; on Android 12
and later they move with a direct phone-to-phone transfer, like the
documents.

## Vehicle photos and documents

A vehicle's photo, and the paperwork you keep in its glovebox
(registration, insurance, inspection, receipts), are **copied into
Vektralog's private storage on this phone**, so they open at the roadside
with no signal. No other app can read them and nothing is uploaded.
Vektralog never reads what is inside a document; an expiry date is the one
you typed.

Documents are in the data export you ask for and, on Android 12 and later,
move with a direct phone-to-phone transfer. They are **left out of
Android's cloud backup, the backup folder and the Google Drive backup**, and
they are deleted with the vehicle and when you uninstall the app.

## Backups

- **Android backup:** your phone's own backup may include Vektralog's
  rides, garage and settings like any other app's, under your Google
  account's backup settings. Left out on purpose: your SOS contact, stored
  documents, ride photos, the sign-in details below, when Health Connect first let
  Vektralog read, the weather switch (only a "weather off" goes along), and the backup
  feature's own settings. Android stops
  backing up an app once its data passes 25 MB, roughly 40 hours of rides;
  the Backup screen tells you when that happens.
- **Backup folder (optional):** a folder you pick (on the phone, a memory
  card, or a cloud-storage app you already use) gets a copy of your rides,
  garage and settings after every ride. Vektralog writes only into that
  folder and reads nothing else in it. Not included: photos, documents, your
  SOS contact.
- **Google Drive (optional, where offered):** a copy of your rides, garage,
  fuel and service entries and settings in a hidden app folder in **your**
  Google Drive, which only Vektralog can read. It asks Google for access to
  that folder and nothing else. Not included: photos, documents, your SOS
  contact. Settings > Your data > Backup > Disconnect turns it off and lets
  you delete the Drive copy; uninstalling the app does not delete it. You
  can also remove it at drive.google.com > Settings > Manage apps, and
  revoke access at myaccount.google.com > Security.

## Optional Google sign-in

Off by default, offered only in some builds, and nothing in the app needs
it. It exists so the Drive backup can show you which Google account it is
in. If you sign in, Vektralog stores on this phone your Google email
address, your display name and when you signed in, and uses them only to
label the backup. Google shows its own sign-in sheet; no password reaches
Vektralog. These details are left out of every backup and of
device transfer, so a new phone never arrives signed in as you.
Signing out forgets them and turns the Drive backup off.

## Permissions

- **Location:** see Location above.
- **Bluetooth (optional, auto-record only):** to notice when a device you
  picked connects. No scanning.
- **Notifications:** the recording notification with Pause and Stop, the
  auto-record countdown, the Crash SOS countdown, a warning that a rigid
  mount is shaking the phone, and one-time notices (a ride interrupted by a
  restart, an earlier ride saved).
- **Full-screen alerts (optional, Crash SOS only):** so the SOS countdown can
  show over the lock screen.
- **Start at boot:** to tell you a restart interrupted a ride, and, when
  auto-record is on and the device you chose is already connected when the
  phone unlocks, to start auto-record's cancellable countdown as if the
  device had just connected. It never resumes an interrupted ride, and it
  never starts a recording any other way.
- **Heart rate (optional, where offered):** read from Health Connect; see
  Heart rate from your watch.
- **Battery-optimisation exemption (optional):** so Android does not stop a
  recording mid-ride.
- **Internet:** for map tiles, the backups you turn on and the weather,
  unless you turn it off.

Vektralog has no permission to read your photos or your contacts, to send
SMS itself or to make calls. Photos reach it only through Android's picker,
one choice at a time.

## How your data is protected

Everything Vektralog stores lives in its private app storage, which Android
keeps apart from every other app. Every connection the app makes uses
HTTPS. Android's own cloud backup is encrypted by Android; the backup
folder and Drive follow the security of the storage or account you chose.
Files you export are ordinary files, readable wherever you put them.

## Keeping and deleting

Your data stays until you delete it. Deleting a ride, a vehicle or a
document removes it from the phone, a ride's photos go with the ride, and
deleting a ride also removes it from the backup folder and the Drive
backup. Uninstalling removes
everything on the phone. Ivnoworks holds no copy, so there is nothing to
ask us to delete. Copies you made yourself, exports and backups in your own
storage, are yours to remove.

## Children

Vektralog is not directed at children under 13.

## Changes

A changed policy ships with the app update and is published at this
address with a new effective date.

## Contact

Ivnoworks · contact@ivnoworks.com
