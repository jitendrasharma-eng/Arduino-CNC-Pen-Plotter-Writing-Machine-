# Arduino-CNC-Pen-Plotter-Writing-Machine-
<h1>🖋 Writing CNC Machine</h1>
<p>A simple Arduino-based CNC plotter designed to write or draw text and images on paper using G-code commands. This project demonstrates basic CNC principles and is perfect for beginners exploring embedded systems, robotics, and automation.</p>
<hr>
<h2>📜 Table of Contents</h2>
<ol>
    <li>About the Project</li>
    <li>Features</li>
    <li>Components Required</li>
    <li>Circuit Diagram</li>
    <li>Software Requirements</li>
    <li>Working Principle</li>
    <li>Installation & Setup</li>
    <li>Usage</li>
    <li>Future Enhancements</li>
    <li>Screenshots</li>
</ol>
<hr>
<h2>✅ About the Project</h2>
<p>The Writing CNC Machine is a DIY CNC plotter that uses stepper motors and a servo to move a pen in the X, Y, and Z directions (pen up/down). It converts G-code files into movement instructions for the Arduino, allowing it to draw text and graphics.</p>
<p>Applications:</p>
<ul>
    <li>Drawing shapes</li>
    <li>Writing text</li>
    <li>Educational purposes for learning CNC principles</li>
</ul>
<hr>
<h2>✨ Features</h2>
<ul>
    <li>✔ Arduino-based, low-cost</li>
    <li>✔ Supports G-code files generated from Inkscape</li>
    <li>✔ Uses stepper motors for X & Y axis, servo for pen up/down</li>
    <li>✔ Compact and beginner-friendly design</li>
    <li>✔ Open-source firmware and hardware</li>
</ul>
<hr>
<h2>🔧 Components Required</h2>
<table>
    <tr>
        <th>Component</th>
        <th>Quantity</th>
    </tr>
    <tr>
        <td>Arduino UNO/Nano</td>
        <td>1</td>
    </tr>
    <tr>
        <td>Stepper Motors (28BYJ-48 or NEMA17)</td>
        <td>2</td>
    </tr>
    <tr>
        <td>Servo Motor (SG90)</td>
        <td>1</td>
    </tr>
    <tr>
        <td>A4988 / ULN2003 Driver</td>
        <td>2</td>
    </tr>
    <tr>
        <td>CNC Frame (DIY or 3D Printed)</td>
        <td>1</td>
    </tr>
    <tr>
        <td>Power Supply (12V, 2A)</td>
        <td>1</td>
    </tr>
    <tr>
        <td>Breadboard & Wires</td>
        <td>-</td>
    </tr>
</table>
<hr>
<h2>⚡ Circuit Diagram</h2>
<img width="3277" height="3538" alt="Arduino_CNC_L298D_Wiring_Diagram" src="https://github.com/user-attachments/assets/468af022-8c1a-4e03-a0d4-6d4fd00e23bf" />
<p>Connections Overview:</p>
<ul>
    <li>X-Axis Stepper</li>
    <li>Y-Axis Stepper</li>
    <li>Servo Motor</li>
    <li>Drivers</li>
</ul>
<hr>
<h2>🖥 Software Requirements</h2>
<ul>
    <li>Arduino IDE (to upload code)</li>
    <li>Inkscape (for generating G-code)</li>
    <li>CNC G-code Sender or Serial Monitor</li>
</ul>
<p>Arduino Libraries Used:</p>
<pre>#include &lt;Servo.h&gt;
#include &lt;AccelStepper.h&gt;</pre>
<hr>
<h2>⚙ Working Principle</h2>
<ol>
    <li>Convert text/image into G-code using Inkscape.</li>
    <li>Send G-code commands to Arduino via USB Serial.</li>
    <li>Arduino interprets commands and moves:
        <ul>
            <li>X & Y Axis stepper motors for positioning.</li>
            <li>Servo motor for pen up/down.</li>
        </ul>
    </li>
</ol>
<hr>
<h2>🚀 Installation & Setup</h2>
<ol>
    <li>Clone this repository:
        <pre>git clone https://github.com/your-username/writing-cnc.git
cd writing-cnc</pre>
    </li>
    <li>Upload Arduino Code:
        <ul>
            <li>Open writing_cnc.ino in Arduino IDE.</li>
            <li>Select correct Board and Port.</li>
            <li>Click Upload.</li>
        </ul>
    </li>
    <li>Generate G-code:
        <ul>
            <li>Install Inkscape with G-code extension.</li>
            <li>Convert text/image → Save as .gcode.</li>
        </ul>
        <p>Note: you can use example gcode which provided in this repository.</p>
    </li>
    <li>Send G-code:
        <ul>
            <li>Use G-code Sender or Arduino Serial Monitor.</li>
            <li>Set baud rate to 9600.</li>
        </ul>
    </li>
</ol>
<hr>
<h2>▶ Usage</h2>
<ul>
    <li>Power ON the CNC machine.</li>
    <li>Place paper and fix the pen.</li>
    <li>Send G-code → Watch your CNC write text or draw images!</li>
</ul>
<hr>
<h2>📸 Screenshots</h2>

![img](https://github.com/user-attachments/assets/af8756de-56b0-4bf6-a567-29c809d08253)

<hr>
<h2>🔮 Future Enhancements</h2>
<ul>
    <li>Add Bluetooth/WiFi control</li>
    <li>Laser engraving capability</li>
    <li>Larger writing area</li>
</ul>
