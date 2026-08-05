# Jester v2 Wheel Menu Structure

---

## 0. Root Menu

![Root Menu](../img/jester_v2/main.png)
Opening the Jester menu brings up this new layout:

- **Option 1**: RADIO
- **Option 2**: AIR TO AIR RADAR
- **Option 3**: TID & WCS RADAR
- **Option 4**: AIR TO GROUND WEAPONS
- **Option 5**: NAVIGATION UTILITY
- **Option 6**: CMS & RWR DEFENSIVE
- **Option 7**: TACTICAL IMAGING SET UTILITY
- **Option 8**: CREW CONTRACT UTILITY

---

## 1. Radio Main Menu

![Radio Main Menu](../img/jester_v2/radio_main.png)
**Path**: `[Jester Menu]` -> `Option 1`

- **Option 1**: AN/ARC-182 (Comm Radio)
- **Option 2**: DATA LINK

---

### 1.1. AN/ARC-182 (Comm Radio)

![AN/ARC-182 Comm Radio](../img/jester_v2/radio_1_comradio.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1`

- **Option 1**: USE GUARD (243.000)
- **Option 2**: USE MANUAL
- **Option 3**: USE CHANNEL
- **Option 4**: TUNE MANUAL
- **Option 5**: SELECT CHANNEL
- **Option 6**: SELECT MODE
- **Option 7**: TUNE ATC
- **Option 8**: TUNE TAC

#### 1.1.5. Select Channel

![Select Channel](../img/jester_v2/radio_1_comradio_5selectchannel.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 5`

- **Option 1**: PREV CHANNEL
- **Option 2**: NEXT CHANNEL
- **Option 3**: CHANNELS 1-5
- **Option 4**: CHANNELS 6-10
- **Option 5**: CHANNELS 11-15
- **Option 6**: CHANNELS 16-20
- **Option 7**: CHANNELS 21-25
- **Option 8**: CHANNELS 26-30

##### 1.1.5.3. Channels 1-5

![Channels 1-5](../img/jester_v2/radio_1_comradio_5selectchannel_3channels1-5.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 5` -> `Option 3`

- **Options 1-5**: CH 1 to CH 5

##### 1.1.5.4. Channels 6-10

**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 5` -> `Option 4`

- **Options 1-5**: CH 6 to CH 10

##### 1.1.5.5. Channels 11-15

**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 5` -> `Option 5`

- **Options 1-5**: CH 11 to CH 15

##### 1.1.5.6. Channels 16-20

**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 5` -> `Option 6`

- **Options 1-5**: CH 16 to CH 20

##### 1.1.5.7. Channels 21-25

**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 5` -> `Option 7`

- **Options 1-5**: CH 21 to CH 25

##### 1.1.5.8. Channels 26-30

**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 5` -> `Option 8`

- **Options 1-5**: CH 26 to CH 30

#### 1.1.6. Select Mode

![Select Mode](../img/jester_v2/radio_1_comradio_6selectmode.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 1` -> `Option 6`

- **Option 1**: MODE OFF
- **Option 2**: MODE TR
- **Option 3**: MODE TR/G
- **Option 4**: MODE DF
- **Option 5**: MODE TEST
- **Option 6**: MODULATION MAN FM

---

### 1.2. Data Link Main Menu

![Data Link Main Menu](../img/jester_v2/radio_2_DL.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 2`

- **Option 1**: SET MODE
- **Option 2**: SET FREQUENCY PRESET
- **Option 3**: SET HOST

#### 1.2.1. Set Mode

![Set Mode](../img/jester_v2/radio_2_DL_setmode.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 2` -> `Option 1`

- **Option 1**: TACTICAL DATALINK SYSTEM (TADIL-C / Link 4A)
- **Option 2**: FIGHTER-TO-FIGHTER
- **Option 3**: OFF

#### 1.2.2. Set Frequency Preset

![Set Frequency Preset](../img/jester_v2/radio_2_DL_setfreqpreset.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 2` -> `Option 2`

- **Option 1**: 300.00MHZ (AI F2F)
- **Option 2**: 300.10MHZ
- **Option 3**: 300.20MHZ
- **Option 4**: 300.30MHZ
- **Option 5**: 300.40MHZ
- **Option 6**: 300.50MHZ
- **Option 7**: 300.60MHZ
- **Option 8**: 300.70MHZ

#### 1.2.3. Set Host

![Set Host](../img/jester_v2/radio_2_DL_sethost.png)
**Path**: `[Jester Menu]` -> `Option 1` -> `Option 2` -> `Option 3`

- **Option 1-8**: Dynamic list of AWACS (e.g., OVERLORD 1-1) or Aircraft Carriers in the mission.

---

## 2. Air to Air Radar Main Menu

![Air to Air Radar Main Menu](../img/jester_v2/airtoair_main.png)
**Path**: `[Jester Menu]` -> `Option 2`

- **Option 1**: BEYOND VISUAL RANGE
- **Option 2**: WITHIN VISUAL RANGE

### 2.1. Beyond Visual Range

![Beyond Visual Range](../img/jester_v2/airtoair_1BeyondVR.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1`

> [!WARNING]
> The Beyond Visual Range menu dynamically shifts its options depending on whether the radar is ACTIVE or SILENT. When you command Jester to "Go Silent", the "STT Lock" option disappears (since it requires an emitting radar), and **all other options shift up by one slot**. This means your macro paths will change depending on the radar state!

#### State A: Radar is ACTIVE (Default)

![Radar ACTIVE](../img/jester_v2/airtoair_1BeyondVR.png)

- **Option 1**: STT LOCK
- **Option 2**: SCAN ELEVATION
- **Option 3**: SCAN AZIMUTH
- **Option 4**: TID RANGE
- **Option 5**: RADAR SETTINGS
- **Option 6**: WITHIN VISUAL RANGE (Returns to WVR menu)
- **Option 7**: GO SILENT (Switches to State B)
- **Option 8**: IFF

#### State B: Radar is SILENT

![Radar SILENT](../img/jester_v2/airtoair_1BeyondVR_7gosilence_newmenu.png)

- **Option 1**: SCAN ELEVATION
- **Option 2**: SCAN AZIMUTH
- **Option 3**: TID RANGE
- **Option 4**: RADAR SETTINGS
- **Option 5**: WITHIN VISUAL RANGE (Returns to WVR menu)
- **Option 6**: GO ACTIVE (Switches back to State A)
- **Option 7**: IFF
- **Option 8**: _(Empty)_

_(Note: The submenu paths below are documented based on the default ACTIVE state. If the radar is silent, subtract 1 from the final Option press for all menus except STT Lock)._

#### 2.1.1. STT Lock

![STT Lock](../img/jester_v2/airtoair_1BeyondVR_1sttlock.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 1`

- **Option 1**: TARGET AHEAD
- **Option 2**: ENEMY TARGET AHEAD
- **Option 3**: FRIENDLY TARGET AHEAD
- **Option 4**: CHOOSE SPECIFIC TARGET
- **Option 5**: FIRST TWS TARGET
- **Option 6**: TWS TARGET NUMBER

#### 2.1.2. Scan Elevation

![Scan Elevation](../img/jester_v2/airtoair_1BeyondVR_2scanelev.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 2`

- **Option 1**: AUTO EL AND AZ
- **Option 2**: 15 NM
- **Option 3**: 20 NM
- **Option 4**: 30 NM
- **Option 5**: 40 NM
- **Option 6**: 50 NM
- **Option 7**: 75 NM
- **Option 8**: 100 NM

#### 2.1.3. Scan Azimuth

![Scan Azimuth](../img/jester_v2/airtoair_1BeyondVR_3scanazimuth.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 3`

- **Option 1**: CENTER
- **Option 2**: RIGHT 20
- **Option 3**: RIGHT 40
- **Option 4**: RIGHT 55
- **Option 5**: AUTO EL AND AZ
- **Option 6**: LEFT 55
- **Option 7**: LEFT 40
- **Option 8**: LEFT 20

#### 2.1.4. TID Range

![TID Range](../img/jester_v2/airtoair_1BeyondVR_4TIDrange.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 4`

- **Option 1**: AUTO
- **Option 2**: 25 NM
- **Option 3**: 50 NM
- **Option 4**: 100 NM
- **Option 5**: 200 NM
- **Option 6**: 400 NM

#### 2.1.5. Radar Settings

![Radar Settings](../img/jester_v2/airtoair_1BeyondVR_5radarsettins.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 5`

- **Option 1**: AUTO
- **Option 2**: TRACK WHILE SCAN AUTO
- **Option 3**: TRACK WHILE SCAN MANUAL
- **Option 4**: RANGE WHILE SEARCH
- **Option 5**: TARGET SIZE SWITCH
- **Option 6**: TARGET ASPECT SWITCH

##### 2.1.5.5. Target Size Switch

![Target Size Switch](../img/jester_v2/airtoair_1BeyondVR_5radarsettins_5targtetsizeswitch.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 5` -> `Option 5`

- **Option 1**: NORMAL
- **Option 2**: LARGE
- **Option 3**: SMALL

#### 2.1.8. IFF

![IFF](../img/jester_v2/airtoair_1BeyondVR_8IFF.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 8`

- **Option 1**: INTERROGATOR MODE
- **Option 2**: MASTER MODE
- **Option 3**: TRANSPONDER MODES
- **Option 4**: M3 CODE
- **Option 5**: M1 CODE

##### 2.1.8.1. Interrogator Mode

![Interrogator Mode](../img/jester_v2/airtoair_1BeyondVR_8IFF_1interogator mode.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 8` -> `Option 1`

- **Option 1**: MODE 4A
- **Option 2**: MODE 4B

##### 2.1.8.2. Master Mode

![Master Mode](../img/jester_v2/airtoair_1BeyondVR_8IFF_2mastermode.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 8` -> `Option 2`

- **Option 1**: OFF
- **Option 2**: STBY
- **Option 3**: LOW
- **Option 4**: NORM
- **Option 5**: EMER

##### 2.1.8.3. Transponder Modes

![Transponder Modes](../img/jester_v2/airtoair_1BeyondVR_8IFF_3Transpmode.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 1` -> `Option 8` -> `Option 3`

- **Option 1**: M1
- **Option 2**: M2
- **Option 3**: M3A
- **Option 4**: MC
- **Option 5**: M4

### 2.2. Within Visual Range

![Within Visual Range](../img/jester_v2/airtoair_2withinVR.png)
**Path**: `[Jester Menu]` -> `Option 2` -> `Option 2`

- **Option 1**: CANCEL HOT RWS
- **Option 2**: JETTISON DROP TANKS
- **Option 3**: BEYOND VISUAL RANGE (Returns to BVR menu)

---

## 3. TID & WCS Radar Main Menu

![TID & WCS Radar Main Menu](../img/jester_v2/tidwcs_main.png)
**Path**: `[Jester Menu]` -> `Option 3`

> [!NOTE]
> Options 1, 2, and 4 in this menu dynamically toggle their text labels based on their current active state.

- **Option 1**: EXPAND TID / COLLAPSE TID (Toggle)
- **Option 2**: ENABLE AUTO EXPAND / DISABLE AUTO EXPAND (Toggle)
- **Option 3**: TID RANGE (Leads to same submenu as 2.1.4. TID Range)
- **Option 4**: TID GROUND STABILIZE / TID AIRCRAFT STABILIZE (See 3.4 below)
- **Option 5**: RADAR SETTINGS (Leads to same submenu as 2.1.5. Radar Settings)

### 3.4. TID Ground Stabilize

![TID Ground Stabilize](../img/jester_v2/tidwcs_4groundstab.png)
**Path**: `[Jester Menu]` -> `Option 3` -> `Option 4`
_(Note: This submenu only opens if Option 4 says "TID GROUND STABILIZE". If the menu currently says "TID AIRCRAFT STABILIZE", clicking Option 4 will instantly toggle it back to the default state without opening a submenu)._

- **Option 1**: 15 S
- **Option 2**: 30 S
- **Option 3**: 60 S
- **Option 4**: 120 S
- **Option 5**: INDEFINITE

---

## 5. Navigation Utility Main Menu

![Navigation Utility Main Menu](../img/jester_v2/navigation_main.png)
**Path**: `[Jester Menu]` -> `Option 5`

- **Option 1**: STEERING MODE
- **Option 2**: SEQUENCING
- **Option 3**: BDHI STEERING
- **Option 4**: SELECT DESTINATION WAYPOINT
- **Option 5**: DIRECT-TO WAYPOINT
- **Option 6**: SELECT SURFACE TARGET WAYPOINT
- **Option 7**: FLIGHT PLAN
- **Option 8**: BULLSEYE / NAV GRID (Toggle)

### 5.1. Steering Mode

![Steering Mode](../img/jester_v2/navigation_1steeringmode.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 1`

- **Option 1**: EGI FLY-TO
- **Option 2**: DESTINATION

### 5.2. Sequencing

![Sequencing](../img/jester_v2/navigation_2steeringsequencing.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 2`

- **Option 1**: AUTO
- **Option 2**: OVERFLY
- **Option 3**: MANUAL

### 5.3. BDHI Steering

![BDHI Steering](../img/jester_v2/navigation_3BDHIsteering.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 3`

- **Option 1**: FLY-TO
- **Option 2**: FP WAYPOINT (Opens Select BDHI Waypoint menu)
- **Option 5**: HUD SYNC

#### 5.3.2. Select BDHI Waypoint

![Select BDHI Waypoint](../img/jester_v2/navigation_3BDHIsteering_2BDHIwp.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 3` -> `Option 2`

- **Options 1-8**: Dynamic list of waypoints (e.g., 01 DEST PRI01, 02 AUTO HB HB, 03 AUTO BE BULLSEYE)

### 5.4. Select Destination Waypoint

![Select Destination Waypoint](../img/jester_v2/navigation_4selectwp.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 4`

- **Options 1-8**: Dynamic list of waypoints (e.g., 01 DEST PRI01, 02 AUTO HB HB, 03 AUTO BE BULLSEYE)

### 5.5. Direct-To Waypoint

![Direct-To Waypoint](../img/jester_v2/navigation_5directtowp.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 5`

- **Options 1-8**: Dynamic list of waypoints (e.g., 01 DEST PRI01, 02 AUTO HB HB, 03 AUTO BE BULLSEYE)

### 5.6. Select Surface Target Waypoint

![Select Surface Target Waypoint](../img/jester_v2/navigation_6selectsurface tgt.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 6`

- **Options 1-8**: Dynamic list of waypoints (e.g., 01 DEST PRI01, 02 AUTO HB HB, 03 AUTO BE BULLSEYE)

### 5.7. Flight Plan

![Flight Plan](../img/jester_v2/navigation_7flightplan.png)
**Path**: `[Jester Menu]` -> `Option 5` -> `Option 7`

- **Option 1**: LOAD FLIGHT PLAN
- **Option 2**: RELOAD CURRENT FLIGHT PLAN
- **Option 3**: MANUAL ENTER WAYPOINT (L/L)
- **Option 4**: MANUAL ENTER WAYPOINT (MGRS)
- **Option 5**: WAYPOINT FROM MAP

---

## 6. CMS & RWR Defensive Main Menu

![CMS & RWR Defensive Main Menu](../img/jester_v2/CMS-RWR_main.png)
**Path**: `[Jester Menu]` -> `Option 6`

- **Option 1**: CMDS MODE
- **Option 2**: MANUAL PROGRAM
- **Option 3**: INHIBITS
- **Option 5**: RWR DISPLAY TYPE
- **Option 6**: SET JAMMER XMIT

### 6.1. CMDS Mode

![CMDS Mode](../img/jester_v2/CMS-RWR_1CMDSmode.png)
**Path**: `[Jester Menu]` -> `Option 6` -> `Option 1`

- **Option 1**: OFF
- **Option 2**: STANDBY
- **Option 3**: MANUAL
- **Option 4**: SEMI
- **Option 5**: AUTO
- **Option 6**: BYPASS

### 6.2. Manual Program

![Manual Program](../img/jester_v2/CMS-RWR_2manualprog.png)
**Path**: `[Jester Menu]` -> `Option 6` -> `Option 2`

- **Option 1**: PRG 1
- **Option 2**: PRG 2
- **Option 3**: PRG 3
- **Option 4**: PRG 4

### 6.3. Inhibits

![Inhibits](../img/jester_v2/CMS-RWR_3inhibits.png)
**Path**: `[Jester Menu]` -> `Option 6` -> `Option 3`

- **Option 1**: INHIBIT CHAFF
- **Option 2**: INHIBIT FLARE
- **Option 3**: INHIBIT 01
- **Option 4**: INHIBIT 02
- **Option 5**: INHIBIT RWR
- **Option 6**: INHIBIT MWS
- **Option 7**: INHIBIT JAMMER

### 6.5. RWR Display Type

![RWR Display Type](../img/jester_v2/CMS-RWR_5RWRdisplay.png)
**Path**: `[Jester Menu]` -> `Option 6` -> `Option 5`

- **Option 1**: NORMAL
- **Option 2**: AIRBORNE INTERCEPTOR
- **Option 3**: AAA
- **Option 4**: UNKNOWN
- **Option 5**: FRIENDLY

---

## 7. Tactical Imaging Set Utility Main Menu

![Tactical Imaging Set Utility Main Menu](../img/jester_v2/tacticalimagingset_main.png)
**Path**: `[Jester Menu]` -> `Option 7`

- **Option 1**: TURN OFF
- **Option 2**: SOURCE: [CURRENT] (Opens Recording Source menu)
- **Option 3**: START RECORDING
- **Option 4**: SNAP
- **Option 5**: SEND

### 7.2. Recording Source

![Recording Source](../img/jester_v2/tacticalimagingset_.2recordingsourcepng.png)
**Path**: `[Jester Menu]` -> `Option 7` -> `Option 2`

- **Option 1**: PILOT
- **Option 2**: RIO
- **Option 3**: RASTER

---

## 8. Crew Contract Utility Main Menu

![Crew Contract Utility Main Menu](../img/jester_v2/crewcontact_main.png)
**Path**: `[Jester Menu]` -> `Option 8`

- **Option 1**: SET INACTIVE (Toggle)
- **Option 2**: SET NO TALKING (Toggle)
- **Option 3**: SET EJECT BOTH (Toggle)
- **Option 4**: DISABLE LANDING CALLOUTS (Toggle)
- **Option 5**: ENABLE AUTO EXPAND (Toggle)
- **Option 6**: DISABLE AUTO VID (Toggle)
- **Option 7**: TREAT NO-REPLY AS BANDIT (Toggle)
