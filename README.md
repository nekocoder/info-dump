info-dump
=========

place for me to drop my stupid ideas
--
[Hacking Game ("System Defense", "Children of "?)]

Goal
> Connect to target core. Take control. 

Main mechanic(s)
> deploy and fortify information obstacles
> probe and take control of enemy information obstacles.

resources
> single-use drones [specialization;specialization]
> multi-use drones [multi-function, moderate stats; mid/high tier]
> Barriers [resists junk data; slows down data transmission one way]
> Sensors [passive observation; can't initiate action on own]
> ping []
> junk data transmission [can overwelm structures; can cause bottle necks, easily trips alarms] 
> data injection [can infiltrate and engage systems; higher chance of revealing your own systems]

random ideas
> DNS server communication
-- (Defense) server reset; clears connections
-- (offensive) server control; discover system location, redirect traffic to you.
> DDOS (causes lose of connection with one or more of one's own systems)
> preset set ups that come with immutable initialization times vs immediate resource creation and use
> processor speed stat that speeds up object creation
> storage speed stat as experience
> Ram speed stat that increases increases initialization speed

Game Flow
> Character cores appear
> imminent attack notice appears (match start)
> initialization starts
-- Free placement if not initializing
> Main Action
-- Create Unit 
-- Destroy Unit
-- Fortify Unit
-- Reposition Unit
-- Give Command
> Win Condition
-- Core has been compromised

Objects
> Drones
-- Attack Drone (sends junk data to slow and disrupt functions)
-- Infiltration Drone (utilizes command injection for hacking or recon)
> Sensors
-- Will relay traffic and object status to a certain point (e.g. DNS, Core)
> Barriers
-- Trash collector (blocks junk data)
-- Input cleaner (checks for command injections)
-- Adaptive (will attempt to check for both)
> Misc
-- Decoys (will respond to commands)
> Core
-- Character's main system (can do many of the same functions as the drones, and even better, but has a higher de-facto vulneralbility)

Example Interactions
> Attack Drone/Trash Collector 
-- AD sends junk data
-- TC receives data 
-- TC recognizes and destroys junk data
-- If TC can't accept a transmission, it will forward (as opposed to crashing)
XX--- If TC is overwelmed (it intercepts each incoming data transmission) it shuts down and must be rebooted
> Attack Drone/Input Cleaner
-- AD sends junk data
-- IC receives data 
-- IC runs junk data and crashes
> Infiltration Drone/Trash Collector
-- ID sends command injection
-- TC receives data
-- TC runs command, gets no error and forwards transmisison
> Infiltration Drone/Input Collector
-- ID sends command injection
-- IC receives data
-- IC recognizes command, checks blacklist and discards data
