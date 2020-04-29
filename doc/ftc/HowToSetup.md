# How to set up the Stream Dream Rig for FIRST Tech Challenge events

## Before the event

It's important to do all the homework in advance, as it can be hard or impossible to run the event if some of the requirements aren't met, and may be difficult to track down the right people or the right answers on the day of the event.

* Coordinate with the event operator and venue owner to ensure the [Venue Requirements](VenueRequirements.md) are met
* Copy all media files necessary for the event to the streaming computer, and set them up in OBS, if possible

## Before set up

The event name and way hosts are referred to in particular can be pretty specific. Make sure you get it right so that everyone is happy. Make sure you know where everything will be happening so that the stream works well, and you're not in the way.

* Ensure you know the exact names of things:
  - The exact event name as it should be displayed
  - The event host's name or preferred way they are listed
  - The location of the event (exact city, etc.)
* Collect the WiFi password from the venue
* Find out the layout of the competition fields, scoring tables, etc.
* Locate the projector(s) to be used
* Ask about the audio system in use and its inputs

## Set up the Stream Dream Rig

* Ensure any tablecloths the event organizers desire are in place
* Place the Stream Dream Rig on the table
* Remove the flight case lids
* Connect the main power cable to an available outlet
* Unpack and connect the monitor
* Position the keyboard and mouse in a comfortable location
* Power on the UPS

## Set up the audio mixer and microphones

Setting up the audio system is one of the bigger wildcards in a venue setup, and may require some quick thinking. Doing this first ensures you have the maximum time available to work out the kinks, and also makes the microphones available for announcements while setup of the rest of the equipment is completed.

### Set the audio mixer to "safe" settings

The goal here is to get the audio system up and running, and configured properly, without risk of damaging the venue PA system. 

* Ensure "POWER ON" (main power) switch is in "off" position
* Ensure "PHANTOM ON" (48V phantom power) switch is in "off" position
* Reset the configuration for channels 1, 2, 3, 4, 5/6, 7/8:
    * Move all sliders to the bottom position
    * Press all "MUTE" buttons
    * Set all "PAN" (black) knobs to center position
    * Set all "AUX 2" / "FX POST" (orange) knobs to "-∞" (fully left, off) position 
    * Set all "AUX 1" / "MON PRE" (red) knobs to "0" (center) position 
    * Set all "EQ" (blue: low, med, high) knobs to "0" (center) position 
    * Set all "COMP" (light blue) knobs to "0" (left) position
    * Set all "GAIN" (black) knobs to "0" (left) position
    * Un-press all "LOW CUT" buttons
    * Un-depress both "LEVEL" buttons for LINE IN 5/6 and LINE IN 7/8 
* Move "ALT 3-4" slider to the "0" position
* Move "MAIN MIX" sliders to the "0" position
* Un-depress "2-TR/USB TO MAIN" button
* Un-depress "2-TR/USB" and "ALT 3-4" "SOURCE to PHONES/CTRL ROOM" buttons
* Depress "MAIN MIX" "SOURCE to PHONES/CTRL ROOM" button
* Set "PHONES/CTRL ROOM" knob to left horizontal position (pointing at the arrow)
* Set "AUX SENDS" knobs to "-∞" (fully left, off) position
* Set "STEREO AUX RETURNS" knobs to "-∞" (fully left, off) position

### Turn equipment on

* Turn on audio mixer by moving "POWER ON" (main power) switch to "on" position
* Turn on each wireless microphone receiver by holding the power button for 1 second
* Connect headphones to 1/4" "PHONES" jack

### Set up "blue" announcer wireless microphone (channel 1)

* Put on headphones
* Turn on the microphone by holding its power button briefly or flipping its power switch
  - Ensure LED on microphone comes on
  - Ensure display on correct wireless receiver comes alive
* Move slider for the channel to the "0" position
* Adjust "GAIN" knob while checking main mix level LED bargraph until speaking peaks around "0"
* Adjust headphone volume to comfortable level using "PHONES/CTRL ROOM" knob (not the sliders!)
* Turn off the microphone by holding its power button briefly or flipping its power switch

### Set up "red" announcer wireless microphone (channel 2)

* Follow the same steps as above for the "blue" announcer wireless microphone, but using channel 2 and the "red" microphone instead.

### Set up the audience wireless microphone (channel 3)

* Follow the same steps as above for wireless microphones above, but using channel 3 and the wireless lapel microphone instead.
* Place microphone aside for installation on the front camera tripod later.

### Set up the (optional) wired microphone (channel 4)

(This is of questionable utility, as a wired microphone near the scorekeeping table tends to pick up a lot of extraneous conversation.)

* Follow the same steps as above for wireless microphones above, but using channel 4 and the wired microphone instead. (Note: The wired microphone may require significantly more gain than the wireless microphones do.)
* Install the microphone in an appropriate location, such as on the table, or a microphone stand.

## Patch into the audio system

For output to the venue audio system, the line-level 1/4" TS *AUX SENDS* port "2" is used. Mixing from each channel to this output is controlled (independently from the main mix) by the _orange_ colored mixer knobs. The main output level is controlled by the orange "AUX SENDS" knob labeled "2". 

There are two ways to connect the mixer's output into the venue audio system: a "Line" input or a "Mic" input. They differ mainly by the expected input voltage (the "level"), with "line level" being 1 V peak-to-peak (p-p) and "mic level" being ~0.1 V p-p. If a line-level output is connected to a mic-level input it will be _exceedingly_ loud and could even damage the speakers. If a mic-level output is connected to a line-level input, it may be so quiet as to be completely unusable.

### Option 1: Connecting to a "Line" input

Connecting to a "line" input is typically best as connecting another line-level mixer output is exactly the expected use for this input. The voltage levels are higher, which is better for longer cable runs, and should be subject to less distortion. These will typically be labeled "Line" or "Line In" and will often be a 1/4" TS (unbalanced mono) jack, sometimes a 1/4" TRS (balanced mono), or an XLR (balanced mono) jack. If available, a balanced connection via XLR should be used.

* 1/4" TRS to XLR adapter
* XLR cable
* XLR to 1/4" TRS adapter

### Option 2: Connecting to a "Mic" input

Sometimes the audio system at a venue isn't set up for external connections at line level, but may have an available microphone input (or, alternately, an existing microphone input can be unplugged temporarily). These connections are almost always via an XLR (balanced mono) jack.

* 1/4" TRS to XLR adapter
* line-level attenuator or "direct box"
* XLR cable
* XLR to 1/4" TRS adapter

### Tip: Connecting long XLR runs with RJ45

In many cases, the venue's PA system's line or microphone inputs may be a considerable distance away from the desired location of the Stream Dream Rig. Instead of long XLR cables, standard Ethernet cables can be used along with XLR to RJ45 adapters on each end of the cable, especially at line level. This can be convenient as appropriate-length cables may already be available, and if not, Ethernet cables are easy to terminate on-site as necessary.

### Connect to the venue audio system

* Set the "AUX SEND 2" (orange) output level to "-∞" (off)
* Locate PA system and identify connection options
* Set the appropriate input level knob/slider on the venue audio system to its minimal/off setting
* Connect an appropriate series of cables/adapters to the venue audio system to the audio mixer "AUX SENDS 2" output (see below) 
* For each announcer microphone, set the "AUX 2" (orange) knob to the "0" position

### Perform an initial test and level setting

* Turn on one of the previously set up and tested wireless microphones
* Set the venue audio system's input level to a low/minimal setting (just barely above the "off" or "-∞" setting)
* Slowly and carefully adjust the "AUX SENDS 2" output knob while speaking into the microphone until your voice is heard through the PA system
* Adjust venue audio system's input level until the volume is approximately correct when the audio mixer's "AUX SENDS 2" output knob is at the "0" position

Note: If the volume is way too LOUD or way too QUIET, and proper adjustment seems impossible, the connection may be at the wrong level ("mic" instead of "line" or vice versa) – see below and adjust as appropriate.

## Turn on the computer

* Power on the computer by pressing the power button
* Log in
* Connect to the correct WiFi network for the streaming using the PCIe wireless adapter
* Connect to the correct WiFi network for the scorekeeper using the USB wireless adapter
* Run a speed test to check for upstream bandwidth of at least ~8 Mbit
* Check that Twitch.tv is reachable
* Connect to VPN if necessary

## Set up field cameras

For each field:
* Expand (13') tripod base but do not raise tripod
* Install tripod adapter and ball mount
* Mount camera on ball mount
* Position tripod at field, centered at the back of the field, but not touching the perimeter walls
* Tape the tripod legs to the floor
* Connect camera with Ethernet cable
* Aim the camera (sharply down and approximately level)
* Raise the camera to its full height
* Make a loop of Ethernet cable 1-2 feet in diameter at the base of the tripod 

## Set up front camera and audience microphone

* Expand (10') tripod base but do not raise tripod
* Install tripod adapter and ball mount
* Mount camera on ball mount
* Position tripod at the front of the venue, and centered reasonably
* Tape the tripod legs to the floor
* Connect camera with Ethernet cable
* Aim the camera (sharply down and approximately level)
* Raise the camera to just above adult head height
* Make a loop of Ethernet cable 1-2 feet in diameter at the base of the tripod 

## Perform cable management

* Leave a 1-2 foot loop of Ethernet cable at the base of the tripod (to take up any forces from tripping on the cable or otherwise and allow a bit of repositioning of the tripod or camera without re-taping the wire)
* Tape the Ethernet cable to the floor neatly
* Coil and neatly hide the remaining Ethernet cable

## Connect to the scorekeeper for score overlays and rankings

TODO: Document this.

## Configure OBS Studio for the event

* Open the OBS Studio application
* Open an appropriate _Profile_ for the event
* Ensure all cameras and input sources are working
* Edit the _Event Information Overlay_ and other informational overlays as appropriate 
* Adjust scenes to have appropriate cropping, centering, etc. as appropriate

## Start streaming!

* Press the "Start Streaming" button in OBS
* Start the `stream-output-xxx` systemd service as appropriate (e.g. `stream-output-twitch-firstnevada`)
* Ensure the stream comes alive on e.g. Twitch using another computer