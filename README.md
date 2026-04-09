# Dual-Rail-Breadboard-Power-Supply-5V-3.3V-
A compact, reliable power regulation module designed specifically for prototyping on standard MB102 breadboards. This project converts a 12V DC barrel jack input into stable 5V and 3.3V rails with high-current capability and protection.

Engineering Architecture:

The system utilizes a linear regulation topology to ensure low-noise power delivery for sensitive analog and digital components.

1. Primary Regulation: Uses the LM7805 to drop 12V down to a stable 5V rail.
2. Secondary Regulation: An LM317 adjustable regulator is utilized for the 3.3V rail, configured with a precision resistor divider.
3. Mechanical Integration: The PCB is custom-shaped with "wings" and bottom-mounted male headers to plug directly into the power rails of a standard breadboard.

Technical Highlights:
1. Power Management: Supports a 12V DC input via a standard barrel jack with an integrated physical toggle switch for hard power-off.
2. Net Class Optimization: Configured specific KiCad net classes for power_input and power_output with increased track widths (0.35mm) to handle higher current density and reduce resistive voltage drops.
3. Signal Integrity: Strategically placed 10µF and 0.1µF decoupling capacitors (C_1, C_2, C_3) at regulator inputs and outputs to suppress high-frequency noise and prevent oscillation.
4. Visual Feedback: Integrated an LED power indicator with a 560Ω current-limiting resistor for immediate status verification.
5. Design for Manufacturability (DFM): Minimum clearance set to 0.25mm to ensure high yield.
