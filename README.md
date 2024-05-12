# Control Technician's Troubleshooting Checklist
Factory Electrician's/Control Technician's Troubleshooting Checklist  
Machines may be different but they are for the most part made of the same components and perform logic.  
So following this checklist when things go wrong should lead the technician to the source of the problem even when the machines are unfamiliar.  

It may not be possible to diagnose a machine failure under lockout/tagout conditions.  
If the machine is unfamiliar, be sure to work with machine operators that know how the machine moves and where dangerous potential energy is captive in the machine which might be relased during troubleshooting.  

1.  #### Ask: Initial Survey.

    1.  Watch, Look, Listen, Smell, Ask, Think, Look at your notes,
        Think again. Don’t just start doing random things.

    2.  What is the problem specifically?

        1.  What is the machine supposed to be doing that it’s not
            doing,

        2.  or what is the machine doing that it shouldn’t?

        3.  What machine parts are expected to move?

    3.  Where are the controls for starting the desired behavior?

    4.  Where are the controls for stopping the desired behavior?

    5.  Where are the troublesome components: air supply, oil supply, water supply, steam supply, fuses, circuit breakers, relays, contactors, PLCs, HMIs, control panels, motors, VFDs, pumps, actuators,
        cylinders, bearings, valves, solenoids, sensors, limit switches, encoders, resolvers, transducers?

    6.  Did anything happen just before this problem appeared?

    7.  How will I know when this problem is solved?

    8.  Has this happened before? What is normally done when this
        problem occurs?

    9.  Do I need to fix this or does the supervisor just want to run
        right now? What will just get them going?

    10. Are all the controls set properly?

    11. Suspect that the answers given are likely incomplete and or
        incorrect. Resist the temptation to just do random things that
        operators tell you to do unless they can explain why they think
        it will solve the problem.

    12. Look at the indicator lights on the operator’s panel? Do they
        show errors?

    13. Are there any error messages at the control panels, computer
        consoles, HMI screens, or VFDs? Pay special attention to the error
        messages which were generated first on the list because these
        may trigger the latter error conditions. Remember that not all
        error messages are representative of the conditions that trigger
        them.

    14. Look for red lights inside the electrical cabinet. Red lights
        are usually bad. Sometimes fuse holders provide a red light to
        indicate a blown fuse.

2.  #### Mechanical issues: Most issues, even those which appear to be electrical turn out to be mechanical. So let's look at the mechanical first.

    1. Loose or broken mechanical connections:
        > Is the motor cool and does it move easily when controls are activated?  
        > Does the motor not move the load?  
        > Look for loose gears, loose set screws, broken belts, broken chains, broken shear pins, and broken couplings.  
        > Check for worn out keyways and missing keys, worn out or misadjusted clutches and brakes, leaking seals at cylinders and valves.  
        > Check that electrically operated clutches are engaging.  

    2. Jammed mechanicals:
        > Is the motor and or the bearings hot?  
        > Does the motor strain when controls are activated or not move at all?  
        > Check fuses and circuit breakers first if the mover appears dead or if single phasing is suspected.  
        > Then look for material jams.  
        > Look for loose bolts or bolts which have fallen out and for loose parts which have shifted and consequently jammed.  
        > Check for worn out bearings.  
        > Check that pneumatically or electrically operated brakes are releasing.  
        > Check that mechanical parts are receiving lubrication and are not seized.  

    3.  Basic Pneumatic issues:  
        > Does the machine have air?  
        > Where are the manually operated valves for air?  
        > Where are the pressure regulators?  
        > Check that air valves are open and that regulators are set to the correct pressure.  
        > What about oil for the air lines?  
        > Does the automatic oil dispenser have oil in the cup?  
        > Lack of lubrication for air operated devices is a huge source of problems.  
        > Listen for air leaks, broken air hoses, broken seals at pneumatic cylinders.  

    4.  Basic Hydraulic issues:
        > Is there hydraulic oil in the reservoir?  
        > Is the pump turning? (broken coupling between motor and pump?)  
        > Is the oil too hot? (Blockage at relief or check valves? Are they stuck?)    
        
    5.  Advanced Hydraulic Troubleshooting. Much applies to pneumatics as well

        1. Caution!
           > Pneumatic equipment can move with explosive speed. Stay clear!  
           > Hydraulic oil under pressure may come out with enough force to sever limbs.  
           > Even when the pump is off the oil may be pressurized by an accumulator or by a heavy load on the hydraulic cylinders.  
           > Hot oil burns   
           > Oil injection injuries usually result in amputation.  
           > So when opening hydraulic fittings: use tools, keep hands clear of fittings, and watch for falling loads as oil is released from cylinders.  
           
        2. Excessive noise?  
            > Air in the system? Perhaps there is air in the system from having been run dry.  
            > Cavitation Noise? Perhaps obstruction between tank and pump causing vacuum at pump input?    
 
        3. Is the pump turning? 
            > Coupling between motor and pump hot? (careful)  
            > Probably broken coupling or slipping on a bad spline so pump not turning.  
            > Why did the coupling fail? Pump hard to turn? Why?    

        4.  Is the pump pumping?
            > Pump is getting unusually hot? Oil unusually hot? Couplings to motor are breaking? Pump is hard to turn by hand?   
            > Suspect a bad check valve at pump output or other obstruction.  
            > Open a connection at the pump outlet to see if oil is being pumped.  
            > Be very careful – oil under pressure is very dangerous.  
            > Even when the pump is off the oil may be pressurized by an accumulator or by a heavy load on the hydraulic cylinders.   
            > It is very dangerous to loosen fittings when the pump is on and also when it is off because of burns, oil injection injuries, and falling loads.   
            > Point hose in a safe direction (maybe back into the tank) when turning on the pump and hold on tight and be ready to turn the pump off.  
            > Consider that excessively hot oil may slip past seals in cylinders because of reduced viscosity.  
            > So finding the source of excessive heat may solve other apparent problems.   

        5.  Getting Flow: No problem with pump and motor  
            1.  Check for signal and solenoid problems.  
                > Actuate the valve manually under load by pressing the recessed button on the valve if available.  
                > If this moves the load reliably, then we know that the trouble is the signal or solenoid. See the next section [Signal or solenoid is suspect](https://github.com/johnshearing/ControlTechniciansTroubleshootingCheckList/blob/main/README.md#signal-or-solenoid-is-suspect)  
                > If there is no movement or movement is unreliable then the problem is not signal or solenoid – it may be hydraulic or it may be a jam.
                > After checking for a jam, see the section [Signal and solenoid are OK, Check for hydraulic problems](https://github.com/johnshearing/ControlTechniciansTroubleshootingCheckList/blob/main/README.md#signal-and-solenoid-are-ok-check-for-hydraulic-problems)  

            2.  #### Signal or solenoid is suspect.

                1.  Listen to the solenoid when switching on and off.  
                    > There should be some sound as the valve moves.  
                    
                2.  Notice if the solenoid is unusually hot.  
                    > Maybe a short circuit in the solenoid.  

                3.  Take a voltage reading with probes at each end of the coil while the control for signal is on.  
                    > There should be full voltage when energized and none when de-energized.  
                    > This proves signal, but still there could be an open in the solenoid.  
                    > So disconnect the leads and compare resistance across the solenoid to a known good solenoid   
                    > Or check for appropriate amperage going through the solenoid when operating.  
                    > No voltage difference across the solenoid could indicate lack of signal, a short in the coil or a broken common.  
                    > In that case disconnect the solenoid and check for voltage between the hot wire and the common when switched on.  
                    > Voltage between hot and common wires would indicate good signal, good common, but a shorting coil in the solenoid. So change the solenoid.    
                    > If there is still no voltage between hot and common then check for voltage between hot and a known good common or go directly to the common terminal of the power supply.  
                    > If there is voltage now then you know you have a broken common otherwise it’s a shorted coil.
                    
                4.  If there is no access to the normal signal voltage:
                    > Then apply voltage to the solenoid with a power
                    supply, battery, or by pig tail or try swapping it
                    out for a new one.

            4.  #### Signal and solenoid are OK, Check for hydraulic problems.

                1.  If the load does not move when valve is actuated manually:
                    > Then the trouble is one of the following:  
                    > a. Valve is stuck  
                    > b. Lack of oil pressure at the valve input  
                    > c. Lack of oil pressure at the actuator input  
                    > d. Blown out seals in the cylinder or actuator   
                    > Check for blown out seals on cylinders before checking valves so as to prevent miss-diagnosing a valve as the problem.  

                2.  Check for damaged seals in the cylinder  
                    > Oil may be leaking past seals instead of moving the load.  
                    > If oil is coming out of the exhaust when the piston is at full stroke or when not moving then the seals must be damaged.  
                    > To test, open the hose connection at the cylinder input to check that there is oil pressure and flow.  
                    > If there is no flow then your problem is back at the valve or in the hose.  
                    > Assuming there is flow, return and tighten the hose connection at the cylinder input and open the connection at the exhaust.  
                    > Turn on the pump again.  
                    > When the piston reaches full stroke or when it stops moving, there should be no oil coming out of the exhaust.  
                    > If oil is coming out the exhaust when the piston is at full stroke then the seals are damaged.   
                    > If everything checks out so far, then there is probably a jam at the load.    
                    > Disconnect the cylinder from the load.  
                    > Then attempt to move the load and the piston independently to see if either are jammed. 


3.  Electrical issues: [Review safety talk here](https://github.com/johnshearing/ElectricalSafety/blob/main/README.md)

    1.  Basic Power issues:  
        > Does the machine have power?  
        > Is the machine plugged in?  
        > Where are the Disconnects, Fuse Boxes, Electrical Cabinets, Power Switches, Fuses, Breakers, and Overloads?  
        > Look these over.
        > If there are no obvious problems then check with a voltmeter starting with power terminals coming into the machine.   
        > Exercise overloads while power is off – sometimes this helps when contacts and aux contacts are worn.  
        > Suspect loose wires at terminals or loose terminal blocks.  

    2.  Basic Heat issues:  
        > Are the electrical parts too hot?  
        > Are Motors, Wires, Connections, Fuses, Power supplies, the PLCs, or the VFDs too hot?  
        > Check with an IR camera.  
        > Open doors and find ways to move air.  
        > Blow dust out of drives and heat exchangers.  
        > Tighten connections. Replace fuses.  

    3.  Control issues:  
        > Be sure to make an [initial survey](https://github.com/johnshearing/ControlTechniciansTroubleshootingCheckList/blob/main/README.md#ask-initial-survey) and then check for [mechanical issues](https://github.com/johnshearing/ControlTechniciansTroubleshootingCheckList/blob/main/README.md#mechanical-issues-most-issues-even-those-which-appear-to-be-electrical-turn-out-to-be-mechanical-so-lets-look-at-the-mechanical-first) first.  
        > Most times an issue that seems electrical will turn out to be some mechanical problem.  

        1.  Check First:
            > Ensure that all the controls are set correctly.  
            > Make sure all switches are in the operational positions.  
            > Check for error messages or error lights at the PLCs.  
            > Check for error messages or error lights at the VFDs.  
            > Check for error messages at the HMIs.  
            > Check for error messages at the computer console.  
            > It never hurts to just clear the machine, power down, and reset.
                   
        2.  Has Power But Won't Start  
            > Where are the Estops and Safety Gates?   
            > Pull out E-Stops and ensure that all safety gates are closed.  
            > Look at the lights on the safety relay(s) to be sure the safety circuit is in the (OK Ready To Run) state.   
            > Measure the voltage on the safety circuit and on the safety relay(s) to be sure the safety circuit is in the (OK Ready To Run) state.  

            > Check the master relay which powers the system after all safety conditions have been met.  
            > Is the master relay getting signal from the safety relay(s)?  
            > Are all the contacts on the master relay closing?  

            > Operate the control or switch for the desired behavior.  
            > Then check the lights on the PLC.  
            > If no input on the PLC lights up when pushing the start switch then we have a problem with the switch circuit.  

            > If no output on the PLC lights up when pushing the start switch then we have a logic problem – all conditions for activation have not been met.  
            > Are all other interlocked machines required by the PLC logic online and are the connecting relays functioning?  
            > Where are the limit switches, photo eyes, reflectors, proxes, encoders, and other types of sensors?  
            > Clean these and check that they are secure, dry, unbroken, functioning, focused,
            > in the correct position, obstructed or not as needed, not picking up unwanted reflections,
            > not picking up or being blocked by intermittent obstructions caused by mechanical failures or
            > lose parts nearby, actuated or not as needed, and that the target is painted as required or that reflectors are clean.  
            > Check that wiring is secure, connectors are seated, and terminal screws are tight.  
            > When replacing sensors, ensure that settings on the new sensors are the same as settings on the old.  
            > Look for power lights and fault lights on PLCs, Power supplies, VFDs, Communications modules, HMIs and Computer Consoles.      
            > Check the ladder logic if possible with a Laptop PC to see what conditions are not being met.   
            > Suspect bad input or output cards on PLC.  
            > It never hurts to turn power off and back on again if any kind of control issue is suspected and exercise all overloads while the machine is off as well.   

        3.  #### When machines move erratically, move uncommanded, stop uncommanded, won’t move, move at a speed unexpected, or lack a starting signal:  
            > Check that photo eyes and reflectors are clean.  
            > Check that sensors, reflectors, limit switches are adjusted and or focused properly.  
            > Check if unwanted reflections are confusing photo eyes.  
            > Check for faulty or broken sensors and limit switches.  
            
            > Check for broken wires on sensors.  
            > If the signal wire is broken but the power and common wires are good then the sensor will appear to function but no signal will arrive at the PLC or relay.  
            
            > When changing sensors, be sure to note original position.  
            > Leave stop nuts in place so as to know the correct placement of new sensor.  
            > Take photos, mark wires, and make diagrams before disconnecting devices.  
            > If possible, remove and replace only one wire at a time.  
            
            > Are limit switches hot (temperature)? Water inside switches?  

            > Check that encoders, sensors and limit switches are fastened securely.    
            > Dithering (erratic motion) is a sign of loose encoder.  
            > If encoder is tight then suspect faulty encoder.  
            > Dithering can also be caused by dirty photo eyes and intermittent sensors.  

            > Check that limit switches are not actually up against their limits.  
            > If a machine won’t move in either direction and nothing else seems to be wrong then consider the possibility that both in and out limit switches are activated at the same time.  
 
            > Important! While taking proper safety precautions, follow the wires. Pull and wiggle connectors. Check that all electrical connections (Power and Signal) to sensors, limit switches, encoders, terminal blocks, PLCs, VFDs and motors are tight and secure. If strange behavior cannot be explained then check for loose electrical connections before giving up and saying I need to look into the PLC. Looking into the PLC will not likely expose loose intermittent electrical connections.  

            > Check that input and output cards are seated securely.  
            > Check input and output lights on the PLC. Compare these against photos taken when the system is ready to run.   
            > If PLC inputs and outputs are bypassed using multiplexers then check the lights on the multiplexers.  
 
            > Check the manual for troubleshooting tips and look at the wiring diagrams.
            > Look over the ladder logic in the documentation.  

            > Check the ladder logic if possible with a Laptop PC to check the state of the PLC.  
            
            > Set up a Watch Application on your Laptop to monitor the state of suspect inputs and outputs of the PLC.  
            > Use the Watch Application to catch intermittent events which are too fast to catch with the human senses.  
            
            > Use the slow motion video function on your smartphone to record machine operation. Maybe you will observe something under slow motion which is not visible at normal speed.
            
            > Use an infrared camera if available and look for unusual sources of heat.  
            > These could indicate jams, clogs, leaks, loose wires, faulty electronics and more.  

            > Check the health of the motors:  
            > Measure voltage, freq, power factor and amperage on all legs loaded and unloaded.  
            > They should be equal.  
            > Voltage, Amperage, and resistance measurements intended to determine the health of a motor must be made at the motor without any connections to brakes, contactor coils, load balancing devices etc.  

            > Check that connections to VFDs are secure and that the drive is functioning correctly.  
            > Check input voltage and output voltage.  
            > Use the meter’s low pass filter (if available) when measuring the output of a VFD.  

            > Check for proper voltages from power supplies and from source power.  
            
            > Call the manufacturer  

        4.  Fried components:  
            > Ask what devices are being energized at the moment your components are being fried?   
            > Ladder logic and electrical schematics should be consulted.  
            > Disconnect all those devices.  
            > Next disconnect the components which are getting cooked and replace with dummy loads on each wire coming in.  
            > Appropriately sized light bulbs and fuses are perfect for this.  
            > Finally, energize the devices one at a time until fuses start blowing.  
            > The blown fuses will lead you to the shorting component.  

        5.  Shorted Motors:

            1.  Short circuits in DC Motors:   
                > Check all rotor windings for shorts and opens at the commutator.  
                > They should all have the same resistance.  
                > Then place one probe between each of the windings on the rotor and the other probe on the stator winding(s).  
                > Then test both of those to the thermocouple and to the ground.  
                > All of these should be open circuits.  

            2.  Short circuits in AC motors:  
                > Check for single phasing (voltage at T1, T2, and T3). Check for equal resistance between all three windings.  
                > Keep in mind that winding resistance must be checked right at the motor with all other wires completely disconnected.  
                > If the brake is included in the measurement then resistance will not appear to be the same on all the windings.  
                > The same holds true when checking amperage.  
                > If the brake is active and the wire being measured goes down stream to the brake as well as to the winding then it will appear as if amperage measurements on that winding are greater than on the other two.  


        6.  If there is a momentary loss of power (for just a second or less):  
            > Often when pushing a button or starting a process.  
            > Usually 24 volt systems but sometimes 110 too.  
            > This is most likely a short circuit.  
            > This may seem odd if no fuse is blown and nothing is tripped out but this is often how 24 volt systems short out.  
            > If it happens when actuating a button then check the input circuit first by disconnecting the button circuit from the PLC and actuating the input with a jumper.  
            > If the problem is still there then the problem is likely on one of the PLC output circuits although there is a small chance that an input activated right after the button is pushed could be the perpetrator.  
            > To find which one, remove output wires on the PLC one at a time while replacing the previous until the problem disappears.  
            > Then it is a simple matter of running down the short.  

        7.  When motors are not moving:  
            > If motor has an electrically powered brake:  
            > Be sure the brake is releasing when the motor is energized.  
            
            > If motor is powered by a VFD:  
            > Check for error messages on the VFD    
            > Check that there is power to the VFD  
            > There should be equal voltages between all three supply side terminals.  
            > Check that the safety circuit on the drive is in the (OK Ready To Run) state.  
            > Run the drive manually using the controls on the drive or put a start signal on the drive.  
            > Check that the VFD is providing the correct voltage to the motor between all three legs when pressing the start button on the machine.  
            > Use the meter’s low pass filter (if available) when measuring the output of a VFD.  
            > There should be equal voltages between all three terminals going to the motor.  
            > Check if motor runs when bypassing the VFD and wiring to a contactor instead.  
            > Swap out the drive with one identical and loaded with the same parameters.  

            > If the VFD is not providing power to the motor when pressing the start button then check that the VFD is getting a run signal when pressing the start button.  
            
            > If no signal:  
            > Broken signal wire? Check for signal at the source (relay, PLC output, ethernet signal)  
            > Remote into the PLC with a laptop. Check the ladder logic to see if the drive is getting a run signal.  
            > Remote into the VFD with a laptop. Check to see if the drive is getting a run signal.  
            > Skip to the section [When machines ... lack a starting signal:](https://github.com/johnshearing/ControlTechniciansTroubleshootingCheckList/blob/main/README.md#when-machines-move-erratically-move-uncommanded-stop-uncommanded-wont-move-move-at-a-speed-unexpected-or-lack-a-starting-signal) for more ideas.  
            
            > If VFD is getting signal and seems to be working, skip to the section [If motors and actuators...](https://github.com/johnshearing/ControlTechniciansTroubleshootingCheckList/blob/main/README.md#if-motors-and-actuators-are-moving-in-one-direction-but-not-at-all-in-the-other)  
            
            > If motor power comes from a contactor:  
            > Check that there is power voltage between all three supply side terminals of the contactor.  
            > Check if contactors are getting signal voltage across the contactor's coil when pressing the start button on the machine.  
            > If no signal, skip to the section [When machines ... lack a starting signal:](https://github.com/johnshearing/ControlTechniciansTroubleshootingCheckList/blob/main/README.md#when-machines-move-erratically-move-uncommanded-stop-uncommanded-wont-move-move-at-a-speed-unexpected-or-lack-a-starting-signal) for more ideas.  
            
            > Assuming you have signal:  
            > Check individual contacts on the contactor with a voltmeter.  
            > There should be no voltage difference between the supply side and the motor side contactor terminals for each leg when the contactor is energized.  
            > There should be power voltage between all the power terminals and ground of course because the contact terminals are energized.  
            > Alternatively, disconnect all wires on the contactor except for the coil wires and check for continuity between the supply side and the motor side contactor terminals for each leg of the contactor when the coil is energized and when not.   
            > There should be continuity when energized and none when not energized.  
            > There should be a change in continuity on axillary contacts when changing from energized and not depending on whether or not the contact is normally open or normally closed.  

        8.  #### If motors and actuators are moving in one direction but not at all in the other:  
            > Suspect a problem in the limit switch circuit or perhaps machine is up against a limit switch and should not be moved.  
            > Problems with a limit switch are very likely if a machine part has become loose or moved out of alignment.  
            > Also check that aux contactors on reversing contactors and overloads as well are working.  

        9.  If there is at least some movement in both directions:  
            > More than likely a jam.  
            > Also consider the possibility that a set screw, key, or pin is missing between a gear and shaft.  
            > This would explain some movement until power transmission is required.  

        10.  Check brushes if applicable that they are seated properly and that they are not worn out.
  
        11.  If overloads or VFDs are tripping, if fuses are blowing:  
             > Reset or replace protector and try again.  
             > If protection does not trip right away, then observe the motor and the load.  
             > See if anything is jammed or binding.  
             > Check for phase imbalance while running (max 2% voltage deviation from average between all three legs and max 10% current deviation on each leg).  
             > Check power for harmonics (crest factor should be 1.4).  
             > Cables from VFDs to motors should be as short as possible in order to reduce harmonics.  
            
             > Be sure the protector in question corresponds with the malfunctioning motor:    
             > It is possible, due to mislabeling or other confusion, that the protector you are resetting has nothing to do with the motor you are working on.  
             > So check continuity on the wires going from protector to motor if there is doubt about which motor a protector is controlling.    
             > Here is how: Turn off all power (lockout/tagout) when making this test for safety and to avoid false continuity readings caused by phantom voltage.  
             > Disconnect wires from the motor in question.  
             > Join the ends of the three power wires coming to the motor from the protector at the motor with a wire nut so that checking continuity can be accomplished right at the protector.  
             > There should be continuity between all three wires at the protector when the wires are joined at the motor and there should be no continuity between the wires when the or wire nut is removed.  
             > In this way you are sure which motor the protector is connected to.  
             > Replace the wires at the motor exactly as they were.  
             > Do not replace the wires at the protector yet.  
 
             > Check that the protector is functioning:  
             > With the protector still disconnected from the motor, press the start button.  
             > If the protection still trips while unloaded then replace the protector.   
            
             > If the overload does not trip when unloaded (when disconnected from the motor):  
             > Check for single phasing: Is the protector providing voltage to the motor on all three legs?  
             > Check voltage between outputs T1, T2, and T3 at the protector.  
             > Voltages should be equal (all within 2% of the average).  
             > If one of the legs is not getting voltage then very likely there is a blown fuse up stream.  
           
             > If all is good at the protector then the problem is downstream towards the motor.  
             > Check resistance between the three wires at the protector going to the motor.  
             > These wires should all be connected together through the windings of the motor.  
             > These are the same three wires you disconnected from the protector.  
             > If there is an electric brake on the motor then you will need to disconnect that brake from the motor windings before making this test.  
             > The resistance should be equal between all three wires going to the motor.  
             > If not, suspect opens or shorts on the motor windings or on the wires going to the motor.  

             > If a problem is detected from above then we need to determine if the problem is with the wires going to the motor from the protector or if the problem is with the motor windings.  
             > Testing the wires going to the motor for shorts:  
             > Disconnect the three wires at the motor. They are already disconnected at the protector.  
             > Now check resistance between the three wires. It should be an open circuit.  
             > Then check the resistance between each of the wires and ground. This should also be an open circuit.  
             
             > If wires going from the protector to the motor don't have any shorts then we need to check that none of the wires are broken:  
             > Disconnect the three power wires at the motor.  
             > Join the three wires from the protector at the motor with a wire nut. Not the motor wires, but the wires going to the motor from the protector.  
             > Check continuity between all three wires at the protector end of the wires.  
             > This will identify which wire (if any) is broken.  

             > If the wires from the protector to the motor have checked out good then we need to check the motor windings for unequal resistances between windings (AC) or across windings in the case of DC motors.  
             > Also check that there is no short between the windings and the case or ground wires.  
             > Remember to completely disconnect the motor from the rest of the circuit including the brake circuit, if any, and measure right at the wires going to the windings.  
            
             > If there are no conclusive results and the problem can not be found then maybe these are failing under load only in which case our previous test will not find the problem.  
             > Replace motor or actuator and replace the protector (contactor, overload, VFD) as well and try again.  

11.  Jumping out NPN and PNP Sensors

    1.  Pull the sensor wires out of the cabinet after marking them and
        jump the PLC input Hi or Low as required.

    2.  To say it in greater detail: Brown is usually Positive, Blue is
        usually Negative, White is usually Signal for NPN, Black is
        usually Signal for PNP. So for PNP sensors, install a jumper
        from where the black wire of the sensor was connected (the PLC
        input) to where the Positive Brown wire was connected so as to
        source voltage to the input. The input in this case is obviously
        a sinking input because it provides a path with a load for the
        sourced voltage from the sensor to drop across as it works its
        way to the negative side of the power supply.

    3.  So for NPN sensors, install a jumper from where the white wire
        of the sensor was connected (the PLC input) to where the
        Negative Blue wire was connected so as to sink voltage from the
        input. The input in this case is obviously a sourcing input
        because it provides a voltage with a load for said voltage to
        drop across as it works it’s way through the sensor to the
        negative side of the power supply.

    4.  Rather than worrying about what kind of sensor you are trying to
        jump out, it may be better to just measure the voltage at the
        PLC input when it is not connected to anything. If the input
        voltage is almost as positive as the positive side of the supply
        when measured from the negative side then it is a sourcing input
        and so connecting it to the negative side of the supply will
        provide a path for the current to flow as electrons journey from
        one side of the power supply to the other and this will turn the
        input on. If the input voltage at the input is nearly as
        negative as the as the negative side of the supply when measured
        from the positive side then it is a sinking input so connecting
        it to the positive side of the supply will provide the path
        needed for electrons to journey from one side of the power
        supply to the other and this will turn the input on.

    5.  I don’t think there is any harm in using trial and error to find
        which side of the power supply the input is to be jumped to. If
        a sourcing input is jumped to the positive side of the supply
        then nothing will happen - the input will remain off but no
        damage will occur. In the same way, it would not cause any harm
        to jump a sinking input to the negative side of the supply. Be
        careful, however not to accidentally connect the positive side
        of the supply to the negative side of the supply thinking that
        one of them is an input. This actually happened to me when I was
        jumping out an input at some terminal blocks which were not near
        the PLC and so there was no visual way to tell which terminal
        was for the input and which were for the positive and negative
        sides of the supply. In this case it makes sense to check which
        is which using a voltmeter. A sourcing input will be at a
        slightly lower voltage than the positive side of the supply and
        a sinking input will be at a slightly higher voltage than the
        negative side of the supply. So measure at the connection points
        all three possible ways. Two of the connection points will have
        nearly the same potential. The odd one will definitely be
        connected to the power supply. Now measure from the known power
        supply connection (the odd one) to one of the others switching
        the red lead of the meter for the black until the reading is
        positive. If the black lead is on the odd connection then the
        odd connection runs to the negative side of the power supply. If
        the red lead is on the odd connection then it runs to the
        positive side of the supply. Now measure to from the know side
        of the supply to the unknown connections. One of the readings
        will show a slightly greater difference in potential. This is
        the other side of the supply. The lead showing slightly less
        potential is the input to the PLC. This input can be jumped to
        the first discovered side of the supply to turn on the input. As
        a double check to see which of the two undiscovered leads is the
        input: take a resistor which will provide about 7 mA when the
        full voltage available from the power supply is applied. For a
        24 volt supply, this works out to about 3.3K ohms. Now use the
        Amp meter in series with the resistor to make a path between
        each of the unknown connections and the known connection to the
        power supply. The reading with the greatest amperage will be the
        connection to the other side of the power supply and the
        connections with the least amperage will be the input to the
        PLC. Jumping the input to the first known side of the power
        supply will turn the input on.

    6.  I remember shorting a positive wire to the case of the emergency
        pull box on the down stacker. This positive wire must have been
        attached to the input of a PLC and was expecting an NPN sensor
        to sink it to ground to complete the circuit and light up the
        LED in the optocoupler. So be careful what is touched when
        jumping out wires

    7.  The colors mentioned above are not guaranteed on all sensors so
        the following method can be used to identify the type of sensor
        and how the signal wire is being used.

        1.  If there are five wires, then the sensor is most likely
            being used as a relay. One wire will be attached to the
            positive side of the supply (probably brown). One wire will
            be attached to the negative side of the power supply
            (probably blue). The three wires left will be for the relay.
            There will be a common wire, a wire connected to the
            normally closed contact and a wire connected to the normally
            open contact. To find out which is which, disconnect these
            three wires and check continuity while the sensor is dormant
            and then active. Make a map of what was learned. Then
            measure the voltage on the common wire. This is the voltage
            which must be brought to the input of the PLC where the
            normally closed contact was wired if you want the PLC to
            think the sensor is inactive or bring the voltage to the PLC
            were the Normally open contact was wired if you want the PLC
            to think that the sensor is active.

        2.  If there are four wires connected to the sensor then there
            are three possibilities:

            1.  If there are only two wires connected to the sensor then
                the sensor can only be a simple switch which either
                opens or closes when the sensor is activated. As
                mentioned above, this type of sensor must be connected
                to a relay or some other type of load or a short circuit
                will result.

            2.  If there are three wires connected to the sensor then
                there are three possibilities:

                1.  The sensor is PNP (sourcing only)

                    1.  The signal wire will connect with the positive
                        side of the supply when either active or
                        deactivated depending on the sensor.

                2.  The sensor is NPN (sinking only),

                    1.  The signal wire will connect with the negative
                        side of the supply when either active or
                        deactivated depending on the sensor.

                3.  The sensor is a simple switch with an extra wire for
                    ground.

                    1.  Normally these sensors are AC and will have a
                        green wire to ground the case. The other two
                        wires put the sensor in series with the load and
                        must both be either on the positive side of the
                        load or on the negative side but not one on
                        either side because that would cause a short
                        circuit.

                4.  Multimeter tests must be made with the sensor
                    connected to a supply in order to see what kind of
                    sensor it is.

                    1.  Test to see if it is a simple switch first
                        because if it is and the brown and blue leads
                        are connected to the pos and neg sides of the
                        supply, a short circuit will result when the
                        sensor is activated. To avoid this, put a relay
                        coil or other load between the sensor and either
                        side of the supply (a series circuit) so as to
                        act as a load. Check if current is flowing
                        through the circuit. Now activate the sensor and
                        check if current is flowing through the circuit.
                        If no current flows in either case than the
                        sensor is not a simple switch. Once it has been
                        determined that the sensor is not just a simple
                        switch, the brown and blue wires can be
                        connected to positive and negative sides of the
                        supply and the signal wire can then be checked
                        with the sensor activated and deactivated so as
                        to determine if the sensor is NPN or PNP.

            3.  The sensor is PNP (sourcing) only in which case one of
                the two signal wires will source (provide a path to the
                positive side of the supply) when the sensor has been
                activated, and the other will source when the sensor is
                dormant.

            4.  The sensor is NPN (sinking) in which case the one of the
                two signal wires will sink current (provide a path to
                the negative side of the supply) when the sensor has
                been activated, and the other will sink current when the
                sensor is dormant.

            5.  The sensor is both PNP and NPN in which case, one wire
                will sink and the other will source when the sensor is
                either active or dormant, depending on the sensor. Some
                sensors have switches so that you can choose if the
                sensor sinks and sources upon activation or if it sinks
                and sources when dormant.

            6.  It will be necessary to determine what kind of sensor
                you have in order to know how to jump it out at the PLC
                or to replace it with something equivalent in the case
                that no exact replacement can be found. If no datasheet
                can be found then this can be determined with a
                multimeter as follows: First connect the positive lead
                (usually brown) to the positive side of the supply, and
                the negative lead (usually blue) with the negative side
                of the supply. With the sensor dormant, attach one lead
                of the multimeter to the signal wire and touch the other
                lead to the positive side of the supply and then to the
                negative side of the supply. If there is no significant
                difference in the readings then we know that the signal
                wire is not connected to anything. It is not providing a
                path to the positive side nor the negative side of the
                supply. In other words, it is neither sinking nor
                sourcing when dormant. Now activate the sensor and
                repeat the test. If there is a significant difference in
                voltage when touching the positive side of the supply
                then we know that the signal wire is connected to the
                negative side of the supply which is to say that it is
                sinking current. So ground the input of the PLC if you
                want the PLC to think the sensor has been activated or
                do not provide any wire to the input if you want the PLC
                to think the sensor has been deactivated. On the other
                hand, if a significant difference in voltage is measured
                when touching the negative side of the power supply then
                we know that the signal wire is connected to the
                positive side of the supply which is to say that it is
                sourcing current. So wire the input of the PLC to the
                positive side of the power supply if you want the PLC to
                think that the sensor has been activated or do not
                provide and wire to the input if you want the PLC to
                think that the sensor has been deactivated.

13.  Sinking and Sourcing Cards:  
     >  DC Sinking Input Cards:  
     > There is one common terminal which is at 0 volts.  
     > The inputs are at 24 volts when False (unlit) and pulled down to 0 volts when True (lit).  

     > DC Sourcing Input Cards:  
     > There is one common terminal at 24 volts.  
     > The inputs are at 0 volts when False (unlit) and pulled up to 24 volts when True (lit).  
