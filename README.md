# LabVIEW-VIs
PURPOSE <br />
To organize useful LabVIEW VIs.

DESCRIPTION <br />
This repository contains VIs used for various DAQ and real-time control tasks.

DAQ
- 'Cal load cell.vi': reads, filters, and averages load cell data and displays results for calibration.

SIGNAL AND PROFILE GENERATION
- 'Sine signal generator.VI': produces a sine signal and optionally appends a deceleration profile for an input frequency, amplitude, duration, and sampling period.
- 'Chirp signal generator.VI': produces a chirp signal and optionally appends a deceleration profile for an input start frequency, end frequency, amplitude, duration, and sampling period.
- 'PRBS signal generator.VI': produces a PRBS signal, development in progress.

FILE I/O
- 'Create CSV with header.vi': creates a CSV in an input (absolute) or relative directory with input header and file name.
- 'Dequeue and Write to CSV.vi': dequeues elements from an input queue (queue is input to the VI) and writes elements to CSV.
- 'Dequeue and Write to binary.vi': dequeues elements from an input queue (queue is input to the VI) and writes elements to binary. Higher performance than writing to CSV.

MOTION
- 'Set jog parameters.vi': displays a dialog box to prompt user for position and velocity for a desired jog move and displays the value of a variable in the dialog box. The input position and velocity are stored for a subseqent jog move, the jog move is performed by a separate VI. 
- Jog Move.vi': perform a straight line move to an input position at an input velocity.
- 'Reinitialize.vi': a stock LV VI downloaded from examples, reinitializes a connection to an etherCAT motor and drive.
