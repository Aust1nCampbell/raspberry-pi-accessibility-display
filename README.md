# Raspberry Pi Classroom Visual Alert System

This project was created for deaf and hard-of-hearing students at Hixson High School. The goal was to create a visual alternative to the school bell that could alert students to class changes and other scheduled events without relying on sound.

The final prototype used a Raspberry Pi 4 to store the schedule and control two 12 V amber strobe lights through a relay. Staff could program repeating weekly alerts or add events for a specific day, then leave the system running on its own.

## Project Demo

[Watch the visual alert system working](hixson-visual-alert-system-demo-github.mp4)

The demo shows the scheduling interface running on the Raspberry Pi and the physical strobe system responding to the programmed alerts.

## How It Worked

The Raspberry Pi stored the programmed schedule and checked the current time for scheduled events. When an alert time was reached, the Pi sent a GPIO signal to a 5 V relay module. The relay switched the separate 12 V supply powering the two strobe lights, allowing the higher-power lights to be controlled by the Raspberry Pi.

The programming interface was designed so staff could add weekly schedules, add one-time daily events, test the visual alert, and clear saved schedules without needing to edit the program directly.

## My Contribution

My main responsibility was prototyping the **Accept Programming** functionality used to configure the alert schedule. I also helped organize the hardware assembly, configure the Raspberry Pi, and integrate the system into the working prototype.

## Hardware Used

- Raspberry Pi 4 Model B
- Single-channel 5 V relay module
- Two 12 V amber LED strobe lights
- 12 V DC power supply
- Raspberry Pi USB-C power supply
- Female-to-female jumper wires
- Custom 3D-printed PLA enclosure

## Project Results

The completed prototype successfully stored programmed schedules and activated the strobe lights at scheduled times. The system was designed to run mostly unattended after configuration and to continue functioning after being restarted. The working prototype stayed within the project's $400 budget.

## Documentation

The original source code is no longer available, so this repository serves as documentation of the completed project. The original team report includes the design process, hardware specifications, build instructions, testing, cost breakdown, drawings, and team contributions.

[View the Final Project Report](Hixson%20HS%20Visual%20Alert%20System%20-%20Final%20Report.pdf)

## Future Improvements

If I revisit this project, I would like to rebuild the scheduling software, improve the user interface, add easier schedule editing, and make the system easier to configure without connecting a keyboard and monitor directly to the Raspberry Pi.
